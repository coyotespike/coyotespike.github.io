---
layout: post
title: Setting Git to Automatically Back Up My Files
date: 2016-08-27 13:19
# Should be longer than 20 words, so it will appear as post summary
description: A project to organize files into Git, create a shell script to back them up, and make it run automatically.
# tags will also be used as html meta keywords.
tags:
  - programming

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---
<div id="table-of-contents">
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline1">1. The Why's and Wherefore's</a></li>
<li><a href="#orgheadline2">2. Finding git files</a></li>
<li><a href="#orgheadline3">3. Further Organizing Git: A Test</a></li>
<li><a href="#orgheadline4">4. Setting up a new Git folder</a></li>
<li><a href="#orgheadline5">5. Setting up the Shell Script</a></li>
<li><a href="#orgheadline6">6. Scheduling with Crontab</a></li>
<li><a href="#orgheadline7">7. And that's it!</a></li>
</ul>
</div>
</div>


### The Why's and Wherefore's<a id="orgheadline1"></a>

If you woke up to find your house burning, what would you grab as you ran out?
Okay, yes, your children and significant other, but *besides* those?

As a data scientist, programmer, and lawyer, obviously I'd grab my computer, the
caretaker of my personal information and thoughts, my gateway to education and
opportunities.

After all, most of us in the digital age have no valuable papers,
stocks, or bonds lying around (hey, that's just how I imagine life 40 years ago,
okay). If you've followed Marie Kondo's advice, your box of mementos might be
trim and small too.

Relying mainly on one piece of hardware allows unprecedented amounts of
flexibility. That freedom has given rise to all of us (kind-of) digital nomads.
Still, we can do better.

What if the computer dies, or gets lost or stolen? What
if you're traveling across borders and don't want to lug a heavy computer
around? And what if you're aware that the US government claims the right to copy
your hard drive (yes, US citizens too) every time you cross the border? Clearly
they usually don't do that, but still.

My computer isn't what's most valuable to me. The information on it is, and
that's what future-proofing is all about: the ability to hop machines as time
passes. 

So why not give myself even more flexibility by automatically backing up that
information? Ultimately I'd like to create a remote development environment,
accessible from any netbook, but making my information accessible wherever I am,
and safe from local loss, is a great start.

With this system in place, I guess if my house burns down, my hands will be
empty? What about my stash of chocolate chip cookies??

Whatever, let's get started.

### Finding git files<a id="orgheadline2"></a>

First things first: what do I even have lying around on my computer? Going to my
Documents folder in my shell, I enter: `find . -name '.git' -type d`.

This command delivers a long list of Git repos - much more than I thought I had!
Happily, I only see two (mostly empty) nested git folders, whew! I delete these
folders.

### Further Organizing Git: A Test<a id="orgheadline3"></a>

However, I kind of have a problem. I have a lot of git-tracked projects already
underneath my Documents folder, and in the root of my Documents folder I have
files I'd like to track.

As a result, I have two options. I can remove all the git folders at the
"leaves" of my directory structure, and then make a parent git folder with
submodules, under Documents. Or, I can stray into forbidden territory and try to
nest regular git folders in a safe way.

Why is nesting git folders a bad idea?  This can cause issues, as the outer
folder is also trying to track the inner folder. Git submodules are certainly
the way to go if possible, and I'd definitely use them if starting from scratch.

For instance, this [Stackoverflow](http://stackoverflow.com/questions/10205438/can-i-have-a-nested-git-repo-inside-a-git-ignored-folder) thread warns that `git clean -dfx` in the outer
repo will remove the nested repo altogether! I don't plan on running that
command, but let's try it out, just in case.

To test, I `mkdir gittest` and `cd` into it, then create a `subgitfolder`. I run `git
init` in both. In `gittest`, I create `.gitignore`, containing only: `*/*`. This tells
git to ignore all subdirectories, like the subgitfolder I just made,
theoretically preventing them from being cleaned.

In both folders, I create test.txt. I `git commit` in both folders, and now comes
the real test. I run `git clean -f`, which cleans up all untracked files, and also
`git clean -dfx`.

Ah, good: the `subgitfolder` and its file is still there. As a result, I have
confidence that I can make Git ignore nested Git repos safely, even if this
isn't best practice. And so I can track files in Documents, without moving them
or my existing Git repositories.

### Setting up a new Git folder<a id="orgheadline4"></a>

All right, I `git init` in my Documents folder, and set up the Git remote -
Bitbucket has free private repos, GitHub has paid ones for cheap.

Next, I can either set up .gitignore as [explained here](http://stackoverflow.com/questions/987142/make-gitignore-ignore-everything-except-a-few-files), like this:

    # Ignore all files.
    *
    # Ignore all directories.
    */*
    
    # But not this file.
    !To-Do.org
    
    # And not these directories.
    !Writing/
    !Courses/
    # And if the files get moved to a different directory, don't ignore them there either.
    */

Or I can set up my `.gitignore` the other way around, like this:

    # Ignore this file.
    Boring-File.
    
    # Ignore this directory
    BoringDirectory/*

Either way, I make sure that this Git repo will ignore all folders with Git
repos inside them.

### Setting up the Shell Script<a id="orgheadline5"></a>

Now that we're all set up with Git, we need to write a shell script, and then
set this script to run automatically.

We could use this command, `find . -name '.git' -type d`, to find all the .git
folders, then add all their parent directories to an array, and for each one `cd`
into the directory and run `git commit` and `git push`. 

As I've centralized the files I want to track automatically, it's simpler for
me to do this instead:

    #!/bin/zsh
    
    date
    cd /path/to/myDocuments/
    pwd
    git add .
    git commit -m "Automatic backup"
    git push origin master

In the future, I can use [this guide](http://ptrbrtz.net/scheduled-automatic-local-backups-versioning-using-git-on-os-x/) or [this guide](http://www.michaelwnelson.com/2014/02/06/automatically-backup-git-with-cron/) as references if I want to
upgrade my shell script.

Finally, we need to make this script executable - we need to give our computer
permission to run it. You can google this, or run something like `chmod 0700 backupGit.sh`,
which gives you as owner permission to run it.

### Scheduling with Cron<a id="orgheadline6"></a>

Cron is a Unix utility, meaning it's a simple command-line program that does
one thing and does it clearly and well.

To start using, run `crontab -e` on your command line. This will open your crontab
file for editing in vi. You can move down to the bottom of the screen with `:`,
the colon, and then exit with `x`, or save and exit with `wq`. 
See this [great little page](https://corenominal.org/2016/05/12/howto-setup-a-crontab-file/) for more.

And as [this guide backing up to Dropbox](https://eothred.wordpress.com/2010/08/18/git-backup-with-dropbox/) explains, your crontab job should look something like:
`@hourly ID=backupgitrepos nice -n 19 /path/to/script/backupGit.sh >> /path/to/script/backupLog.txt 2>&1`

This command will make Cron run your task every hour (although I used
`@midnight` instead) and then put the log results into a text file.

If struggling with vim is too much for you, put the little crontab script above
into a txt file, then run `crontab <filename>` on the command line.

You can check if Cron has your job with `crontab -l`, which will show all tasks.

### And that's it!<a id="orgheadline7"></a>

All important documents will now be safely stored, automatically and
securely. Naturally I've encrypted private documents as necessary, as we
shouldn't store private information unencrypted, and Org-Mode makes that easy.
