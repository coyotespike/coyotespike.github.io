---
layout: post
title: What's New and What's True
date: 2016-09-19 13:44
# Should be longer than 20 words, so it will appear as post summary
description: At times, programmers' incessant quest for the perfect language or framework can look like time-wasting self-indulgence. In the longer run this leads to good things.
# tags will also be used as html meta keywords.
categories: ["software", "programming", "startups"]

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

### Self-Indulgent Wastes of Time<a id="orgheadline1"></a>

Old-timers and experienced web developers often complain that each new framework
is just hype, just recycled ideas from the past couple of decades. They add
nothing, and there's no reason to continue learning new frameworks except to
speak the same language as their less-reflective colleagues.

This criticism isn't entirely off the mark. We programmers love tweaking and
rewriting things to fit our own computational aesthetics. Especially in a
business environment, we often have to be reminded *not* to re-write the entire
damn codebase. That code *works*, and refactoring definitely will take longer than
you think.

As Rich Hickey notes, programmers know the benefits of everything and the costs
of nothing. Just how large are the benefits of this new language, this new
framework, this new library? Do they justify the costs of setting it up, of
integrating with the surrounding ecosystem, of learning it?

### A Sigh of Resignation<a id="orgheadline2"></a>

One response to this criticism can be a resigned eye-roll. Paul Graham notes
that it's very hard to tell who's a good programmer, but one sign is that
they're finicky about their tools. They just don't like to work with inferior
languages or frameworks or editors, just as a good chef can work with knife but
might insist on Wusthof knives.

Given that fact, we might accept this ceaseless experimentation as the price we
pay for good engineers.

Nevertheless, it's important to emphasize that in the larger picture, all this
frenetic writing is *not* a waste of time.

### The Good Old Days<a id="orgheadline3"></a>

Let's remember that not so long ago the front-end and back-end folks sat in
different rooms, as it were, leading to the traditional diagram "client --
business logic -- database" or Model-View-Controller paradigm.

And not too long ago the front-end was seen as "not real programming," with all
the heavy-duty stuff taking place in the back end. You needed designers and
front-end specialissts, and then you needed sysadmins and you needed back-end
programmers.

Today more and more of the logic lives in the front end - I've had backends that
literally just stored the user's information in Redis and then returned it on
login. All the computations, logic, navigation, etc., took place in the
browser. Stupid backend engineers, what do they know?

These days full-stack web developers are more the norm than the exception. Of
course any larger company or well-established startup will have front- and
back-end specialists, but the distinction isn't nearly as sharp anymore.

### Open Source<a id="orgheadline4"></a>

Part of this story, by the way, goes beyond the specific languages and
frameworks and libraries that actually see a lot of usage, to individual
projects and tutorials which individual developers create for fun and
goodwill. 

This massive community effort, much of it enabled by GitHub, allows newbies to
learn and get up to speed through examples and instruction. The modern open
source movement continue to create astounding wealth by opening the craft of
programming to those without the luxury of learning on the job.

### Sysadmin, and Emacs<a id="orgheadline5"></a>

Just as remarkably, with Docker and Dokku we are starting to see the full-stack
developer extend to the operations side, to server management and system
administration.

Before Docker and Dokku, services such as Heroku enabled solo developers by
taking all of that off their hands. I take the increasing popularity of "DevOps
culture" as another sign that the solo developer will run servers as well.

The same multiplying effect can be seen in tools like Emacs and Org-Mode. I can
efficiently plan and track projects, administer servers, produce reproducible
research, perform polyglot literate programming as in Jupyter notebook, organize
research and writing, format mathematical writing, publish to a blog, and code
in a personally-suited IDE in every language. Of course there are other goodies
like listening to music, because Emacs, but the point is that without this tool
I'd need two of me to do the same things.

### The Bigger Picture<a id="orgheadline6"></a>

Due to the constant rewriting of languages and libraries, today one programmer
can accomplish the work of an Army company of programmers. Famously, WhatsApp,
Mailbox, and Instagram each had astoundingly few employees. Instagram exited
with 13 employees all told, at a market valuation of $100 million per employee.

I'm by no means a demigod or even lesser hero of programming, but by myself, I
can do what 20 programmers would have accomplished about the year 2000. This
churn of technologies enables individual programmers, and thereby enables new
businesses with their own societal innovations to get started.

As many other have noted, just starting a software-based business, which doesn't
even have physical production expenses, cost *millions* only a couple of decades
ago. Then it cost hundreds of thousands. Now if you give me $10k, I and a
co-founder can live on that for 4 months and start a company - and we can do
that because the programming is easier.

Constantly rewriting software to your own specifications may look incredibly
finicky and self-indulgent, and maybe sometimes it is. But it's also the source
of great progress in programming, and therefore also the world.
