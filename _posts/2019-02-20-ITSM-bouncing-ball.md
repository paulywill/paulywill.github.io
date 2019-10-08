---
title: The ITSM Bouncing Ball
date: 2019-02-20 00:00:00 Z
permalink: "/ITSM-bouncing-ball/"
layout: post
comments: true
---

In a previous version of this blog I would throw up random posts that received very little audience attention and more or less for my own amusement. Then I posted one entry that had a massive response and ranked high on the Google results. It was titled, [*"BMC Remedy Sucks! - And Here's Why"*](https://web.archive.org/web/20150302010546/http://paulywill.com/bmc-remedy-sucks).
It was an unfair rant about Remedy specifically when the truth is more procedural and cultural rather than the short comings of a single ITSM solution.

Some of the _joy_ of working in [Github](Github.com), I suspect for some developers and IT professionals, is the straight forward approach of collaborating with others. And although there is a bit of a learning curve, the [Github flow](https://guides.github.com/introduction/flow/) is remarkably easy to follow. In stark contrast is the half-implemented efforts of ITIL procedures with feature overloaded products. 

The frustrating part for any IT professional is being told they have to submit a "ticket" or a "request" and then left to their own devices to figure out how exactly to do that.

> What do you want in this field?

If for example there's a required field with potentially 1000 possible options in a dropdown or paginated results, the minimal effort or default option will ALWAYS be selected. Details will be skipped, documents short and vague, and the whole process and procedure becoming pointless. A Post-It note on my desk is MORE useful than your empty field trouble-ticket.

A control center (ie. Helpdesk) or Operations fixated on _"Closing those tickets!"_, will also put the whole process in contempt. I remind many of my colleagues and those in Operations that the tickets are also our Knowledge-Base that have wonderful search engines attached, and yet if a reoccurring issue keeps happening and the only details are:

```datestamp: THIS broke... now fixed```

Well, what's the point? I take no great joy pointing fingers nor following up with colleagues what that magical fix was, but at some point there should be basic root cause analysis and what was done to resolve the problem. If I'm able I will always include all the related email threads, screenshots, links and commands that were used to fix something. Open source and available for all. Similar to the activity seen on Github.

I also blame the some of the bureaucratic training regarding [ITIL](https://en.wikipedia.org/wiki/ITIL) and similar IT service management "looks good on paper" theories. There was an idea floating around at work that any new entries would have to pass ITIL certification before hire. This unfortunately was not implemented AFAIK, nor were the previous staff in any encouraging way taught ITIL practices. Thus you have some members on the same team confused about the subtle differences between __*'Assigned'*__ and __*'Affected'*__ when opening trouble-tickets, nor why there's a need for tickets at all when email or a phone call has always done the trick.

![My contribution](https://media.giphy.com/media/nJPkKr231dvKo/giphy.gif)

> Keep asking the dumb questions, point out confusion.

You're the user, the IT professional, and the gatekeeper before [GIGO](https://en.wikipedia.org/wiki/Garbage_in,_garbage_out) .

I keep asking and keep cc'ing everyone on the same team what to fill in and why. I make them spell it out for me, and soon it's obvious those ordering the tickets to be created don't really know the nitty gritty details nor care themselves. 

Good questions to ask:
*"How should I open this ticket? What's a good example? Who set this form up and why did they include this field? Which team do I assign it to? Who is affected and following-up? What's the SLA?"*

If I had my way I would push those in charge of the UX to extremely limit the fields and cleanup the options to human consumption or something easily automated to CI/CD in the future. To make it really clear who is holding court and what is required next. 

Basically I would make a bouncing ball for all to follow.




