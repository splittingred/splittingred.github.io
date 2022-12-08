---
title: "Learn the Code"
date: 2014-05-18T13:20:30-06:00
draft: false
tags:
- software engineering
- management
---

A good buddy of mine worked at a software company a few years ago that was moving at a breakneck pace of growth. The
company was doing well, and my friend was on a software development team that was in charge of one of the core parts of
the product. He enjoyed his job, but found that he was never satisfied with his boss. The team always felt overworked,
tech debt rose, and eventually quite a few high-talent engineers left.

What happened?

His boss was a great boss, from a managerial perspective. An old-school SEM (Software Engineering Manager), he had
decades of experience. Held regular 1 on 1's with the team. Was good at keeping the team out of meetings, and provided
the team with lots of context about business decisions. But he had one flaw — he didn’t know the codebase. Or the stack.
He was a native C coder, but the stack they worked on was in Rails, and he’d never picked it up (external hire).

This left him relying heavily on his team for estimates, technical understanding, and implementation details. This
eventually caused the problems above.

## The Changing of Faces
When you move from a team lead position to a managerial role, no one really tells you what’s about to happen. You just
get a new team, are expected to lead it and keep the engineers happy and productive, and off you go. Hopefully you’ve
read up a bit about managing teams, but you probably have some element of leading from your prior gig.

What they don’t tell you is how little time you will have.

If you’re a SEM at a larger company, your weekly schedule will look like an asteroid field of meetings. There will be
precious little time for you to “get in the zone” and crank out solid code. You have new responsibilities — planning new
features, explaining technical limitations/needs for business proposals, HR-related tasks, documentation, reporting and
metrics, etc. These will likely fill around 70-80% of your week, if you’re lucky. That other 30%? If you’re not precious
with it, it’ll disappear too — emergencies, pointless meetings, false alarms. They’ll eat up that free block faster than
a toddler and cake.

So here you find yourself, doing a slew of new tasks, keeping your team happy and meeting deadlines, and finding
yourself slipping further and further away from the code. Some people call this the natural progression of leadership.

I call it short-term thinking.

## You Have To Understand
So much of software engineering these days isn’t creating perfect, mind-blowingly beautiful code. It’s getting a product
to market first. It’s shipping code fast so that you can ensure the company has money for the next month. It’s making
sure your product has the edge over competitors before they get the edge on you — and that means you can’t always have
the perfect solution. You just have to have the right one.

Unfortunately, this often creates miles and miles of technical debt. It’s not uncommon. How companies deal with it will
define their success. But back to you—you’ve been off the code for a few months now, solidly booked in meetings and a
process-driven glaze, and your code-mind is crashed from the sugar rush of your first quarter as an SEM. You’ve missed a
good bit of what the codebase has had added to it. Products change daily; you’re reading digests from weeks ago. Likely
you don’t even know one of your engineers swapped out this one part of the UI framework that changes everything in how
views are now developed. They just told you “we found a way to build views faster by X, Y and Z.” Likely you trusted
them, but have no clue how you would build a New View, and sure don’t have time to figure it out.

So, you start just trusting your engineers. Not inherently a bad thing—but now your tribal knowledge is slipping. When
stakeholders are asking you for high-level estimates on the fly, you’re finding “I’m not sure, let me ask my team” to be
more and more a common response. You are having a hard time even thinking about technical vision for the team — that’s
the Lead’s job, right?

So, so many engineering managers fall into this pattern. And I’d argue it’s where their effectiveness drops like an
anvil.

## Case in Point
Remember that technical debt your team was accruing? Tight deadlines made it so your team had to bend all the rules to
get a project out, and now it’s going to take them twice as long to make something the next time, because they have to
make sure the toothpick tower won’t fall when they start adding more sticks to the top.

But you don’t know this. You just flat out can’t imagine why it takes Greg 4 days to do task X, because when you were an
engineer you could do it in 1 day. Simple. Greg must be poorly skilled, or demotivated, or just doesn’t care.

So, your team starts getting irritated with you. “Death march”. “Slave driver”. “Jerk.” All these are common terms
engineers bluntly have for management that simply doesn’t see the effect of their actions caused by distance from
day-to-day work. It’s not really management’s fault, per se — more the process—but the team doesn’t see that. All they
see is you asking them for something in a day that everyone who’s committed code in the past month knows isn’t possible
in 3, much less 1.

That unknown-to-you tech debt is now killing your team, losing their respect for you, and hurting the company. And
you’re at the helm.

## Get Back to Where You Belong
Flat out: you need to know what your team goes through to build the stuff you ask them to do on a day-to-day basis. And
the only way you can reliably and accurately do that is by being in the code. Picking up (even menial) tasks and doing
them yourself. Your team will respect you if they know you know their pain. They’ll also work harder for you. And will
likely solve pretty much anything you throw at them — because they know people above them know, and have their back.
That’s important.

You’ll also be more effective in estimates for stakeholders. You’ll be able to get time for your team to pay down
technical debt, because you’ll be actually able to tell the company why it’s important that time is made, so that the
company can scale later. And, you’ll be able to stop bad design decisions your team might accidentally make (as all
teams do) because you have knowledge of the systems.

I recommend carving out a portion of your week—some recommend 30%, but I feel you’ll know the number—to coding. Dive
into all the projects you manage. Know how to do basic tasks in them. You don’t have to be an expert on them, nor should
you be. But you should be able to operate in them so if someone asks you how to do X task, you can coherently explain
the technical implementation.

I also recommend not taking high-priority items—remember, 70% of your week is still taken, and that’s your job too. But
there are low-level items you can do to keep your code-mind fresh, and understand the daily slog of a codebase. If you
really want the respect of your team, take the shit work. Nothing motivates an engineer more than a boss taking the
stuff they don’t want to do so that the engineer can work on the fun items.

You’ll find quickly that you’ll soon become a more effective manager. And your team will be better, too.
