---
title: "Why the Way We Look at Technical Debt Is Wrong"
date: 2016-01-19T21:45:03-06:00
draft: false
---

This post is cross-posted from bigeng.io — feel free to read there!

---

I’ll be straightforward at the start of this post: I firmly believe that the most important issue a company deals with
is how it reconciles itself with technical debt. Period.

Now, here’s the real point of this post:

> Technical Debt is a Positive and Necessary Step in software engineering.

First off, let’s define technical debt for the purposes of this post, as the words can mean many different things to
different people. I view technical debt as any code that decreases agility as the project matures. Note how I didn’t say
bad code (as that is often subjective) or broken code. A good example is this: you have, say, a shipping application
that doesn’t have 100% test coverage, has many classes violating SRP, and has poor domain modeling.

That’s not a bad thing. Why?

## The Most Important Thing is Getting the Thing to the User
Startups fail, often. Actually, scratch that. Startups fail, nearly always. The reasons for this are legion, but more
often than not in my experience the reason is speed. Systems take too long to get to market, which causes marketing
efforts to stall or become irrelevant, and competitors beat out the startup to an offering.

Often I meet engineers who want to build their own company where they can “do software right”. They’d build their own
application idea from scratch, doing TDD and 100% test coverage; it’d be widely scalable; it’d have flawless class
modeling; it’d use the latest technologies and have robust APIs; and it’d just generally be a system that any engineer
who laid eyes on it would suddenly fall down on their knees and claim “we’re not worthy!”

This is a flawed worldview.

Tech businesses aren’t successful because they had perfect code and systems. They’re successful because they got a
product to market fast and at the right time. They got out their protoype fast (hacks and all), tested and tweaked it,
and then scaled. It is wholly arrogant to believe you will have a product on first launch that will be widely acclaimed
and quickly adopted. Often it will take fast, iterative changes and tweaks with a small userbase and constant feedback
until the right mix of features and pricing are met, along with aggressive marketing — and then growth happens.

So why do we feel we need to build software in an entirely different way?

Think of it like a city. The most successful cities in the world, such as New York, London, Vancouver, Sydney, etc —
were most definitely not built with populations of millions of people in mind. They were iteratively improved as time
went on and demand grew. Roads were improved. Highways built. Subways and mass transit added. I could go on, but the
idea is the same; as an engineer there is no realistic data point proving that you’ll need to scale to 1,000,000 users
on your first day. So don’t waste time building for that at start.

## Agility, Agility, Agility
Often when discussing tech debt as a strategy, questions come up like, “How are we going to be able to tweak with a
crappy system?” “Don’t iterative improvements need scalable architecture?” These are valid concerns that deserve
thoughtful answers.

And, like most difficult questions in engineering, the answers are mixed. I’m going to posit that there are areas of
your system — and this may vary based on your use case — that shouldn’t need to care about tech debt at all. On the
other hand, there are areas you should guard furiously against accruing large amounts of debt.

The focus on technical debt should be centered around agility.

On your first launch of a product, or feature, or new system, you need to ensure specific parts of that system can
change rapidly. UIs, for example, are often the areas tweaked the most — copy needs changing, move this field this way,
or this form could be streamlined. Integrations with other services via APIs, however, likely stay pretty constant.

For example, in your shipping app above, you’re likely to not change your API integration with USPS or FedEx too much
after the initial connection is built. What you do with the data and pieces may change, but the service bridge itself
will likely stay the same.

So — I’d argue it’s actually OK to accrue technical debt in areas of your application that are not going to change
often. The reason is this:

## Technical Debt is Not Real Debt
Technical debt is only debt in that it hampers agility. Codebases that are poor take more time to develop new features
against. Testing is slower. Switching domain modeling is more painful. Financial debt, however, accrues interest and
hurts more regardless of what it is incurred for.

You can have areas of your application that have significant portions of technical debt for yearsand still not actually
negatively harm the business or product. This is simply because those areas don’t change often, and therefore don’t
actually harm development against them. This is why in large companies you often see services with older language code
that has been untouched for years.

A reminder, here, though — technical debt is not buggy code or systems that are broken. That isn’t technical debt, and
that will harm your product.

Focusing on Agility in Development
So what areas of the application need to keep tech debt balances low to maintain overall business agility? In my
experience, two of the most important ones are:

### User Interfaces

Often these require extensive change and need to be agile enough to embrace change. This is why single-page applications
have grown in such favor over the past few years; they allow quick agility at the UI layer without the need for API
changes.

### Data Structures

As Linus Torvalds once said:

“Bad programmers worry about the code. Good programmers worry about data structures and their relationships.”

This is absolutely true. At the beginning of every project, the most important thing you can do is get your data
structures correct. For instance, if you’re using a relational database, and your models are improperly structured, this
will cause you significant pain later on. If you build a system using NoSQL that later needs to become highly
relational, you will incur massive frustration in the future.

Getting your data structures correct is paramount. Ensure you’ve got that right at first.

### Application Segmentation and Debt
So this is great and all, but how does one actually do this in practice? One easy way is throughsegmentation. Build your
application into siloed areas of concern. One way to do this is through microservices; another is through just
separating your persistence models from your business logic (using service layer or interactor patterns is a great way
to do this).

This keeps areas of your system clean and concerned only with the actions they perform. It also segments technical debt.
That USPS integration? Well, if you have that siloed in a microservice, it doesn’t really matter to the rest of the
larger product if the tech debt is high in it, as long as the interfaces stay consistent. The rest of the product will
perform merrily with rapid changes, and not incur any slowdown because the systems are decoupled.

Furthermore, with regard to testing, heavily test areas of the application you anticipate getting lots of load and
traffic. Test highly probable use cases and unhappy paths. Don’t waste a bunch of time bulletproofing the system on a
use case that’s likely to happen very rarely and that would cause little harm. Always remember the impact and larger
perspective on what you work on. Time is infinitely valuable, so why waste it?

## In Summary
Technical debt is ok, and often a solid product strategy. The importance is getting to market. When launching a new
system or feature, focus your effort and time on areas of the product that need to be agile, and move quickly through
areas that don’t. Later, if the product proves that it can drive revenue, you can revisit those areas and improve if
they need to scale.

Software evolves, and the best software iteratively improves itself to meet demand. It doesn’t start out massively
scalable; it gets there through time and user adoption.

It’s always important to understand the context: there’s no reason to build an eighth wonder of the world if no one’s
going to be there to look at it.
