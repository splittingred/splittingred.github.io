---
title: "The Power of Context in Software Engineering"
date: 2014-30-03T20:57:59-06:00
draft: false
---

It seems like every single company I’ve worked for, or interacted with, is currently striving to find the “10x”
engineer, the rock-star developer, the genius game-changer software architect. Much effort and time are put toward
getting these liberators of success, with companies not only believing but actively spreading the idea that these people
exist, and they are going to get them.

There’s just one small problem. No one really knows what the 10x engineer does, or looks like, or represents. Is it
someone that generates ten times as much SLOC than their peers? Do they deliver projects weeks earlier than others? Or
do they just turn a mediocre team into a passionate, kick-ass development machine that creates products at insane
speeds?

In this post, I’m going to argue that the problem is that we’re looking in the wrong spot. Instead of searching for the
mythical 10x engineer — and making our current employees second guess themselves about whether or not they’re any
good—we should instead be looking on how to improve our own teams, and make them more efficient.

The Power of Context
Context is a strange word. Most people, when they use it, use it almost like an ace kicker in poker: it halts the
conversation, makes the end result clear, makes you wish you had it more often. “Poor George. If only he had more
context, he’d have done that better.” “Can’t you see the larger context?”

But what is context in software engineering, anyway? I’m going to posit that it’s the ability to understand foundation
building versus product shipping. I cannot count the number of engineers I’ve met who feel that they have to have every
single application they build be the Sears Tower before knowing whether it’s even worth being built.

The Failure Principle
Experienced developers — and entrepreneurs—understand that ideas fail 90% of the time. You’ll get an idea, try it out,
and no one will want it and you’ll have to try something else. Repeat, ad nauseum, until one day (or not), something
clicks and your business is formed.

Most engineers, by default, don’t get this. We live in a world of automated testing, of proofed algorithms, of
battle-worn design patterns. Things are supposed to work, and if they don’t, we fix them immediately and ensure they
never happen again through tests.

How does this disconnect affect engineering, then? Aren’t most engineers right to assume that whatever they build should
always be bullet-proof?

I’d argue no, mostly.

Applied Context
Most software projects are going to die, or become obsolete, within 6 months of being written. Anyone can take a good
index of Github to prove this out. An experienced engineer gets this. They build with what I call “applied context” —
make the app just good enough to get some dollars (or movement) behind it, and then if it proves itself valuable, go
back later and bulletproof it. This is one of the main reasons why they move so much faster.

I would argue that most tech startups fail not because their technology isn’t any good, but that they hyper-focus
engineering a perfect solution when one simply isn’t needed. Most ideas don’t need perfection. They need traction. And
the best way to get traction is to hyper-focus on one single use case that you know will turn a profit. Once you’ve got
that, then you scale.

On a more micro-level, I’ve worked with many engineers that spend far too much time making a Da Vinci work of art out of
something that simply didn’t need to be. It just needed to do one use case and be done. Experienced engineers know with
relentless precision where to focus their effort — and don’t waste energy elsewhere. They understand that there are
probably 62,000 other engineers out there have built the same thing they’re doing and are trying to make money off of it
too. And most of those 62k are better engineers than they are.

So what do they do? I believe experienced engineers do the following:

Reuse, reuse, reuse: in today’s distributed packaging world, it’s absurd to build things if a gem/package/composer file
exists for it. Build off of what other people have already done, better than you could have.
V1 the app before building V2: The idea that you should have a super-scalable system before having a paying customer is
ludicrous. Get yourself a paycheck first with a fence before trying to build the Great Wall.
Understand what can be done later: Deadlines are realities. Sometimes you have to make sacrifices in engineering to hit
them, and a seasoned dev knows this — and focuses his work around ensuring that it happens and postponing optional
tasks.
Memorize Big O Notation: This will simply change everything if you understand this. So many engineers want to refactor
every line of code just to reduce SLOC, or make it pretty in some new design fad, but don’t understand that if a 20-line
method has the same Big O as a 2 line method, it may be a complete waste of time to get to the 2 liner.
Build user-first, always: So many developers build from the use case of the developer, rather than the user. They overly
CRUD the system, or build a UI that is absurdly linear. They take forever to ensure that every possible configuration or
endpoint is built. This is a ridiculous waste of time. Similar to TDD — build your single user use case first, and then
fill in the gaps later when that user is now paying you. This is far better than a feature-rich but utterly confusing
system that no one wants to use.
The beauty of these things is that they’re not natural talents. They’re not unique to 10x developers, but they’ll make
anyone produce at 10x speed. They’re simply something anyone can learn.

Focusing on the right context makes you faster. Remove distractions in your development, and get your teams to do the
same, and you’ll be amazed at how you’ve now got a team of 10x developers, for free.
