---
layout: post
title: Review of "Notes on the Synthesis of Form"
date: 2016-06-24 16:50
# Should be longer than 20 words, so it will appear as post summary
description:
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

Today I read *Notes on the Synthesis of Form*, after seeing a Hacker News user 
comment that it's his favorite book, and he totes his dogeard, penciled-up copy 
with him everywhere.

For good reason. Christopher Alexander crafts a conceptual and practical toolset 
for design thinking, and I'm very happy to have it in my cognitive toolkit.
Christopher Alexander's argument, in miniature, goes like this.

Traditional crafstmanship and architecture fits the user's way of life very well;
it had and has very few misfits. (We'll talk about lack of fit rather than fit,
which is more than a semantic quibble, because it's easier to diagnose and fix
problems than it is to design the one-best-way from scratch.)

Traditional architecture worked so well because it was developed over hundreds of
years. Succeeding generations only had to tweak small parts of the design as their
lives changed. The subsystems of the problem - how to live comfortably - evolved
slowly, and thus so could the design.

We no longer have the luxury of "un-self-conscious design." Society changes too rapidly.
Of course, if you ask traditional craftspeople to innovate quickly, they do no better than we do.
People in the past learned to avoid mistakes in architecture through long apprenticships
during which they absorbed the tradition. We have formalized the principles, which allows
us to teach and to learn the practice much more quickly. Formalizing also gives
us a conceptual hierarchy, which is the only way to grapple with the overwhelming
numbers of requirements in our designs.

For instance, if you're going to design a teakettle, you would like it to heat easily,
to hold heat well, to feel good when you pick up, to hold about the right amount of
water, to be easily stored, to not steam up your cabinets, to be easy to clean,
to cost a reasonable amount, and so on. We group these requirements under "economics,"
"safety," "aesthetics."

That sounds like a good thing, but unfortunately we use these concepts just because
they're in the common vocabulary, not because they're particularly well-tuned to the
specifics of the problem at hand. These crudely-cut concepts tempt us to consider
cheapness or safety or whatever but not less-easily-articulated desires, and they
tempt us to optimize the easily-measured, the easily-communicated, the easily-considered.

This is not a good process of design.

To avoid these problems, we can move up another level of abstraction. Write down
every possible requirement you can think of. Try to make them specific, concrete,
and independent of one another. Or, similarly, if you have an existing design,
write down every annoyance or problem you have with it.
Then you can connect these problems or requirements with other related problems.
I have no place to be alone in my house, and also I can hear through the walls too
easily. There's no convenient place to sit with my family, and also the hallways
are too long and winding.

Mathematically, we can consider the list of problems, and the list of their linkages
or relationships, as a set, a graph/network, a tree, or a sort of Venn diagram 
of concentric circles. Although our lists of requirements will start to reveal
the inherent structure of the problem, we should resist the temptation to slap
our old labels on them!

In this way, all the problems, all the things we want, will build themselves up.
We'll begin to see the many subsystems which form the overall system. We can keep
score of which requirements are satisfied or not satisfied (and even for requirements
like price, we still count "cheap enough" or "not cheap enough," to avoid over-optimization).

By using diagrams in this way, we'll be able to manage the overwhelming complexity
of designing from scratch, and we'll be able to solve more of the small problems
and misfits, which when solved make up "good design," a good way of living with
and within man-made structures.

We can see that the structure of the problem itself, and our process of design, 
are deeply linked and must mirror each other.

So much for my brief précis!

This book, and several others of Alexander's, have had large impacts in architecture,
product design, and software engineering.

Why software engineering? Well, "engineering" is a misnomer, as everyone knows.
Alan Turing was perhaps the first to realize that a computer program, which is
written from small pieces of logic embedded in the programming language, will have
unexpected and hard-to-predict behavior. See generally, Conway's game of life, complexity, etc.
But after software programming really got going, managers tried for decades to impose 
the predictable deadlines of normal engineering on it.

Finally we wised up, a bit. Engineering and programming aren't the same, as 
the well-written essay [Abstracting Engineering Away](http://bensu.github.io/abstracting-engineering-away/) explores. Programming and
engineering share a mathematical vocabulary, as well as many design patterns.
Engineering, though, is at least partly a collection of best practices from solved
problems. An engineer faced with a brand-new problem acts a lot like a hacker,
trying this and that. In software, as soon as we've solved a problem, we can abstract
it away, because software is reusable!

For that reason, in software we're far more likely to be designing or re-designing
at a more fundamental level. And that brings us back to design thinking and Alexander.

Alexander's rigorous, detailed, comprehensive method provides context for his later
books which found enthusiastic acceptance in the programming communities. When I
attended Hacker School, now Recurse Center, in New York, I was exposed to idea of
progamming patterns. At the time, it was too much too soon (I've just grokked algorithms
and don't know what a webapp framework is, what the heck this conveyor belt pattern??).

Set within the larger idea of design thinking, and the method for design thinking
which he outlines in *Notes*, software design patterns make much more sense.
So I guess I'd better turn to *A Pattern Language*, and then review [Clojure design patterns](http://mishadoff.com/blog/clojure-design-patterns/)!

As a closing comment, Alexander's focus in *Notes* on subsystems, and the ability to 
fix them, also reminded me of [microservices](https://medium.freecodecamp.com/an-introduction-to-microservices-2705e7758f9#.j0h1vp9pq), which I think of as extending the 
modularity and abstraction we use in the rest of programming.
