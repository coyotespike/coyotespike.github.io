---
layout: post
title: Oracles as APIs
date: 2018-12-24
# Should be longer than 20 words, so it will appear as post summary
description: "A short comparison of web and blockchain development, and the uses of oracles"
# tags will also be used as html meta keywords.
categories: ["blockchain"]

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

### Meet the New Backend - Same as the Old?
One of the nice things about developing blockchain applications is that all of
  our front-end skills apply in this new area of tech. Your React/Angular/Vue
  skills, your UX/UI and CSS skills, you'll use all of those when you build a
  blockchain application.

The difference is that instead of a database or server, you'll put key parts of
  your logic into the blockchain. At a very superficial level, you can think of
  the blockchain as a new server storing your logic and database.

That's very superficial, though, because storing anything at all on the
  blockchain is fantastically expensive. Imagine you've gone back in time to the
  1970s, when programmers had to worry about kilobytes of text. They had to
  delete text generated by one part of their program in order to free up space
  to run the rest of their program!

As a result, you can't even store data structures to iterate over, because you
  cannot store a list that could grow without bound. This is a common mistake that new Solidity programmers make.

### Of Oracles and APIs
As [this](https://www.toptal.com/ethereum/ethereum-oracle-contracts-tutorial-pt1) [series](https://www.toptal.com/ethereum/ethereum-solidity-oracle-contracts-pt2) of [articles](https://www.toptal.com/ethereum/oracle-contracts-tutorial-pt3) on Toptal discusses, the blockchain equivalent of an external API is an oracle.

One interesting point to draw out from this article: yes you must "trust" the oracle, but the oracle is an oracle because of a cryptoeconomic scheme. As a result these new APIs lack a decentralized point of failure - they should be more resilient and reliable. 
  
A blockchain executes code in public. Because you can see what it's doing, you
  don't need to blindly trust that it's doing the right thing. Personally, I
  prefer to say blockchain schemes build trust, instead of removing trust. To
  work together as humans, we need to build trust on many different levels. If
  we can offload some of that trust-building work to the blockchain, we can
  focus on building interpersonal trust and get down to work faster and more
  effectively.

At any rate, the blockchain works because it's backed by cryptoeconomics - that is, we pay
  people with tokens to run it. In the same way, we pay people for reporting
  accurate information to an oracle, and we penalize them for not reporting it.

At the time of this writing, few oracles exist. We'll need many, many more to
  enable all the blockchain applications that we want to build. And we'll want
  to [build a TCR](http://coyotespike.github.io/blockchain/2018/05/05/A-Very-Snobby-Club.html) to curate a list of the best oracles, so that developers can
  look up the best oracles to use as APIs.
