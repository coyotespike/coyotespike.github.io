---
layout: post
title: "An Intuitive Description of the Blockchain"
date: "2016-08-13 12:30"

description: "The blockchain is one of the most exciting software innovations of the decade - a very simple guide to what it's all about."

tags:

- programming

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
# hide QR code, permalink block while printing.
hide_printmsg: false
# show post summary or full post in RSS feed.
summaryfeed: false
---

## A Society Built on Trust<a id="orgheadline1"></a>

For you and I to work together, we need to trust each other. If either of us thinks
we are being cheated, we won't trade goods or services. In person, we can come to
trust each other by personal contact and cues, through a relationship. This gets
harder the larger the group gets, and the less we know each other, and the farther
away we are from each other.

To solve this problem of trust, usually people use some trusted third party. 
For instance, if I am buying shares in your company, then I want to know that you have told me
the truth about how well your company is doing. You show me your financial books,
but that's not enough. An accounting firm, with a public reputation and federal laws
to govern them, comes to check out your books. That third party gives me the confidence
I need to make a decision.

In the case of money, we trust the government and the bank. Every time we swipe
our credit cards, or click "add to cart" on Amazon, we trust that the government
has banking regulations, and that our banks will do the right thing. In turn,
Your local grocery store and Amazon trust that the banks will ensure they get
paid. They don't need to know us personally.

If you and I make a deal, to ensure the other person won't try to change the
terms or back out, we make a big contract, with lots of witnesses signing
it. The contract is hard to fake, and we each have copies. The contract is like
a third party, guaranteeing we can trust this transaction.

Now, if I am selling property, what's to prevent me from selling the same property twice?
In fact, the problem of the same piece of land getting sold twice is a large one, 
and the law has specific rules to deal with it (in Texas, the last good-faith buyer
gets to keep the property, which is very sad if you are the second-to-last buyer). 
To solve this problem, there is a large ledger the government keeps, and
you go to the building there (4th Street in Austin, I think), and write down who got what, when. 
Then your title to the land is secure. This is another way to solve the trust problem.

Whether we use an accounting firm, a government, a bank, a contract, or a big
ledger downtown, we are solving the problem of trust by having a central third
party help us out. This *one person or thing* over there will sit in between us,
so to speak, and help us both ensure the deal is going well.

## Building Trust Without a Middleman<a id="orgheadline2"></a>

However, there is yet another way to solve the trust problem. Suppose instead of
using a contract, or a third person, or something, we all stood around in a
circle, and we wrote down in a ledger in the middle what we agreed to. There'd
be no way to fake that! Doing it in public, with a good record, is an excellent
way to ensure trust. (That is, as long as one of us didn't bribe the majority of
the other people there!)

But we can make this system even better. Suppose instead of one central ledger,
everyone there had a ledger, and copied into their own ledgers whenever someone
announced an agreement. With so many independent records, once we made a transaction, 
there would be a record of it forever.

This way of creating trust is called a distributed ledger system, and today it's
better known as the "chain" in blockchain

And if we just program our computers to keep the ledgers for us, keeping them
will be much easier. Each entry in the ledgers is secured by using cryptography,
which is extremely hard to fake. The entries are announced to everyone in
groups, and those are the "blocks" in blockchain.

Why did no one use this public ledger system before in history? Two
reasons. First, the entries were too easy to fake, but the use of cryptography
now means that they cannot be faked.  Second, it was too easy for one powerful
person to get everyone else in his or her pocket, but the internet is all over
the world, so the computers (which are running this ledger system for us) are
harder to corrupt.

So the first important thing about the blockchain is that it is the first practical
way to have trust between total strangers without a central authority, using this
public ledger. The second important thing about the blockchain is that it can be
run using computers, on their own, automatically.

The first thing people used this new system of trust for, was to make a new money. They
just hooked up that system of trust to a series of math puzzles, cryptography puzzles - 
you got a "bitcoin" for each puzzle you solved, and the public ledger guaranteed that you had
solved it, and you alone, and so the coin could only belong to you. The puzzles got
harder as more of them got solved, to prevent runaway inflation.

But it needn't stop there. People can make other agreements using this system
too - agreements about governing companies, or buying images and movies, or
owning pieces of companies, or checking out a company's books, or just a regular
contract. In fact, just about any agreement, or exchange of goods, which
involves trust, can be done using this blockchain. And because the agreements
can be automated, it might be possible to make a big structure of
mini-agreements. The future might look something like what Vernor Vinge
described in Rainbow's End, where people earn small amounts of money for pieces
of art, or for research, or what have you.

## Difficulties and the Future<a id="orgheadline3"></a>

It is not a perfect system. Even though most of the work is done by computer,
soemtimes an ambiguity arises, which humans can exploit or at any rate have to
deal with. In one famous case, everyone began upgrading to a new set of ledgers,
essentially. Because half the computers were on the new set and half the
computers were on the old set of ledgers, a thief could tell one ledger he had
purchased something and was now legally entitled to it, and tell the other
ledger he hadn't spent any money. He could have his money and spend it too. The
details are still being ironed out.

At any rate, no one really knows what a really successful application of the blockchain
would look like - what the Facebook of the blockchain, making something new and
fun for non-techie people, would look like. But many people are excited about the
idea and working hard to find out. 

And that's the blockchain and BitCoin.
