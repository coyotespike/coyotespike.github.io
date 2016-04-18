---
layout: post
title: Open science: research, equipment, education, data sharing, publication, funding
date: 2016-04-18 15:50
# Should be longer than 150 words, so it will appear as post summary
description: How to become a 'real scientist' as an indie researcher, and how to practice open science 'from farm to market'
# tags will also be used as html meta keywords.
tags:
  - synthetic biology

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline1">1. Open Science</a>
<ul>
<li><a href="#orgheadline2">1.1. Research</a></li>
<li><a href="#orgheadline3">1.2. Equipoment: How to Build a Synbio Lab</a></li>
<li><a href="#orgheadline4">1.3. Education</a></li>
<li><a href="#orgheadline5">1.4. Preregister experiments on the blockchain?</a></li>
<li><a href="#orgheadline6">1.5. Data management and sharing for ongoing projects</a></li>
<li><a href="#orgheadline7">1.6. Open access, post-pub peer review</a></li>
<li><a href="#orgheadline8">1.7. Funding</a></li>
<li><a href="#orgheadline9">1.8. A hypothetical work process</a></li>
</ul>
</li>
</ul>
</div>
</div>

# Open Science

Over the past few weeks I've been intensively researching how best to contribute to the fields of science that interest me.
In the process I've read a lot about the problems and benefits of academic science.

Academic science unites training, knowledge dissemination, funding, and equipment. Most of the world's advances in science
occur in academia, and it remains a good way to get into science.

On the other hand, several folks who have been there and done that have told me there are more efficient ways to get educated
and begin research. More broadly, and concerningly, institutional scientific practice suffers from poor data practices
that lead to inaccurate results - exhibit 1, Ioannidis' conclusions about medical results, exhibit 2, the social science 
reproducibility crisis.

If, like me, you get frustrated when you read about negative results that disappear
due to the "file-drawer" effect, about data hidden by frightened, lazy, or greedy researchers, about papers behind
paywalls, about inefficient scientific education, or what have you, take heart.

The tools for a completely open path to research, equipment, education, data management and analysis, funding,
and publication already exist! While I'll admit I still worry about scaling up research (surely a big academic lab is going to be hard
to beat if you want your research to mean something), this is a very encouraging discovery.

A lot of other people, senior and junior, are thinking about these problems too. There is a broad coalition already
in place. All we have to do is join them.

## Research

This one has recently become much easier. [LibGen](http://libgen.io) is a huge repository of the bulk of scientific research
ever published. If you can't find it elsewhere, you can often find it there. The sister project is [Sci-Hub](http://sci-hub.io),
which uses members' library access to find results, and then donates a copy to LibGen.

## Equipoment: How to Build a Synbio Lab

To get started, take a look at [DIYbio](http://diy-bio.com/diybio-lab-equipment/)'s list, [The Quest for the $500 Home Molecular Biology Lab](http://www.mlo-online.com/the-quest-for-the-500-home-molecular-biology-laboratory.php), [Hackpad's list](https://hackpad.com/ep/pad/static/51UIsplVYrd).
[OpenWetWare](http://openwetware.org/wiki/DIYbio/FAQ/Equipment) has another good list, and here's a slightly older article on [the same quest](http://scienceblogs.com/worldsfair/2009/04/09/using-ebay-to-set-up-a-molecul/).

In addition, here are [two](http://collections.plos.org/open-source-toolkit-hardware) [collections](http://www.thingiverse.com/jpearce/collections/open-source-scientific-tools) of open-source tools.

One of the links on OpenWetWare disrecommends working with live animals for awhile, as the data will be too noisy.

## Education

I'm most excited about [Synthetic Biology: A Primer](http://www.amazon.com/Synthetic-Biology-Paul-S-Freemont/dp/1848168632), and [Synthetic Biology: A Lab Manual](http://www.amazon.com/Synthetic-Biology-A-Lab-Manual/dp/9814579548).
I'll also look at [Draft Primer for Synthetic Biology](http://openwetware.org/images/3/3d/SB_Primer_100707.pdf) and [Principles of Synthetic Biology](https://www.edx.org/course/principles-synthetic-biology-mitx-20-305x).

You can also look around for [good synbio starter projects](http://onlinelibrary.wiley.com/doi/10.1002/bmb.20352/epdf), and - especially - can pick a published result and try to replicate it.

In addition to those and standard molecular biology textbooks, I've become convinced that a high level of statistics knowledge
is essential to do anything worthwhile.

## Preregister experiments on the blockchain?

Suppose an independent or beginner researcher wants to practice open science.
Open data is easy - as Jeffrey Rouder shows, a shell script with git makes automatically backing up data easy.
Proper analysis is harder, but again the math and techniques can't be that hard to figure out.

But how about pre-registration? Using a blockchain to pre-register your experiments would be
the simplest and most flexible approach, as it doesn't require a journal or any institution. You just register
whatever experiment you design and go on your merry way, secure in the knowledge that you've publicly committed
yourself to your experiment. No one can say you changed horses mid-course.

I didn't find any website specifically devoted to pre-registering experiments, though it will probably be easy
just to upload a document to existing blockchain websites.

These websites hash - encode - the contents of the file in such a way that no one can read it, but preserves the identity of your document.
In this way, a blockchain proves your document (for instance, your experiment design) existed at that point in time.

I did find [these](https://db.erisindustries.com/science/2016/03/14/blockchains-and-science/) [two](https://db.erisindustries.com//science/2016/03/15/chains-and-science-how-to/) articles on using the blockchain to store all sorts of data. They seemed more speculative than just
using the blockchain to pre-register, but interesting nonetheless.

## Data management and sharing for ongoing projects

Now suppose I've open-sourced my data, workflow, techniques, and analysis. I publish to an open-access online journal,
I'm commenting on my own work and reviewing others' work on my blog or some other platform. Congratulations, I'm now
Doing Science Openly.

However, a million atomized researchers all working in perfect openness have solved the larger half of the problem
of making science work faster - transparency, reproducibility in principle - yet we now have a search problem.
How do you efficiently find other work, and how do others find (and credit you for!) your work?

[Figshare](https://figshare.com/), [Dataverse Project](http://dataverse.org/), and [Open Science Framework](https://osf.io/) are three pieces of that puzzle.
Figshare and Dataverse function like GitHub in that they are repositories for open data, and
also say they assist with publication venues.

OSF appears to be related to [The Center for Open Science](https://cos.io/). It's a full-fledged scientific project management
platform, which assists in finding and citing other projects.

## Open access, post-pub peer review

[PLoS](https://www.plos.org/open-access/), BiorXiv and rXiv are obvious examples. [eLife](https://elifesciences.org/) looks like a wonderful venue.
<https://thewinnower.com/>
<https://hypothes.is/>

## Funding

[Walacea](https://walacea.com/) and [Experiment.com](https://Experiment.com) both look excellent.

## A hypothetical work process

Having run through all of that, let me throw out a hypothetical path to getting a small yet serious lab up and running.

First, spend a year or so with the synthetic biology Primer and Lab Manual, and other educational 
projects. In this way you'll learn lab techniques, a lot of science, and maybe even start looking for
a project that no one has done yet - original research.

Second, as you self-educate, build open data practices into your workflow. Pre-register, back up your data
and techniques and workflow publicly, make your analysis open.

Third, when you have an original line of research you'd like to pursue, use Experiment.com to get funding.

Fourth, when you have a result worth publishing, use OSF, eLife, BiorXiv, and so on to publish first.
Then look for another open-access venue in which to publish. 

**When you're published, or when someone cites your work, break open a bottle of champagne! You're a real scientist.**
