---
layout: post
title: 
permalink: /form-and-semantics
date: 2021-09-22
# Should be longer than 20 words, so it will appear as post summary
description: Finding causality and contributing without deep domain understanding
# tags will also be used as html meta keywords. Only use one, as it goes in the URL
categories: ["philosophy", "science"]

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

### A Content-Free Approach
You can contribute a lot when you first arrive at a company as a software engineer. If, you're familiar with the technology, and everything is really well-organized, you look around and feel that you know where things are. You know where to start looking, and you know the course the information will take as it flows through the system.

This is a way of saying the system architecture allows you to work on a problem without knowing anything about the problem domain, because if you've just joined a new company as an engineer you might know nothing about the business or users.

For instance, you can immediately start contributing by reviewing PRs for syntax or architecture, or figuring out where info should get piped to. If a feature is really well specified - say it's been groomed and described by other engineers - you can even start making PRs in your first week.

How long can you work on a problem without knowing anything about the domain? This depends on the size of the company and your goals, but in principle indefinitely.

### Debugging as a Formal Approach
When you start debugging a problem, often you have to resist the urge to dive right into the code, hunting for the problem in logic that's causing all this mess. Instead, the correct approach is to zoom out and figure out where in the system the problem is coming from. For example, you can use a kind of binary search, or a differential diagnostic. 

In a binary search, you go to the middle of the whole system flow - whether it's a file or the entire application - and check if you see any errors there. This is especially useful if you code in a functional paradigm, because then you can check the shape of the data at that point. 

Or if you're dealing with a lot of side effects, you can list all the possible failure points and then start with the most likely. This is the differential diagnostic.

Only after figuring out the most likely source of the error do you start thinking through code. In fact, you might never need to think through code. You might just be able to try a few different types of input, and a few different locations for a log, until you find the source of the problem. Then you try nearly-random fixes until it all works. 

You can get very far in debugging by treating the system you're working on as a black box, accessible only by tinkering around the edges and observing behaviour.

Once again, working at the level of logic and architecture only, you can make significant contributions and analysis. This is a purely formal approach, in the sense of paying attention to the form and not the semantics of the problem.

This is essentially how geneticists work, because the systems they work on are so complex and full of feedback loops. Really, the analogy between debugging and doing genetics is a surprisingly strong one.  A geneticist usually finds causality by knocking out a gene and seeing what happens, which is an enormous amount of work, but doesn't establish the mechanism (although biochemistry can partially fill in the blanks).

### A DSL
Still, contributing to a project by working only with logic and data structures and architecture is a sort of shallow approach. Eventually it's helpful have to change gears and start thinking about the semantic meaning of all this data and logic.

The fact that it's so difficult to think through genetic mechanisms - the biological equivalent of working through the semantic meaning of code - is a significant limitation on the field. Part of the appeal of synthetic biology is its promise to increase our ground-up understanding of cellular processes.

As a software application matures, the team writes more and more custom functions and classes, hopefully with well-chosen names, and you use these functions more and more instead of just the built-in language functions. As a result, over time, your application approaches a Domain-Specific Language.

It's littered with functions like `getAllUsersWithSocialAccounts`, which result you feed into `getPostsByAllUsers`, and from there into `displayAllPosts`.

In an application like this, to do any work, you have to learn the domain. You quickly leave the logic-only, architecture-only zone and start thinking about the meaning of the code. What is it trying to do, and why in this particular way? You can only work in the codebase if you understand it.

In other words, built into the language of the codebase itself is a fair amount of domain knowledge. The codebase itself embodies a deep approach rather than a shallow one.

This is also the case in biology, because scientists usually have well-defined jargon which carries a lot of semantic content.
