---
layout: post
title:  "Look Squirrel... Like Development"
date:   2018-04-13 23:19:05 -0400
categories: coding
---

Life is complicated.

As I write this is a busy Tim Horton's (the Canadian café of choice) everyone is juggling conversation between friends, caffeinating themselves, shoving carbs in their food holes, and checking their social status on their digital sidearms... a lot is happening.

We're nothing more than naked apes and busy squirrels.

I'm certainly no exception. Even on a late evening when I want to slowly shutdown the screen and relax, life has other plans.

Sick child. Angry and worn down spouse. And a long list of projects I've created for myself.

Thus the breather and re-group at "the Timmies".

## Rabbit Holes and Can of Worms

In my hopes to get one thing done I'm often "rabbit-chasing" and "something-shiny" distracted off my initial intentions. Sometimes I'm actually able to land the plane.

A great example is preparation for the [AWS Certified Developer - Associate Level](http://awstrainingandcertification.s3.amazonaws.com/production/AWS_certified_developer_associate_blueprint.pdf) exam I have [next month](https://www.timeanddate.com/countdown/generic?iso=20180511T12&p0=1202&font=cursive).While doing some studying I realized needed AWS CLI install on my Mac. Which I thought I had already done in the past.

`Command not found.`

Alright.

`pip install awscli`

And followed by something I've run into before.

```
pyenv: pip: command not found

The 'pip' command exists in these Python versions:
....
....
....
```

This led me down a long trail of trying to troubleshoot the issue with pyenv and why PIP was not working. This is typical in most IT work and development, and thankfully I found the solution: [remove pyenv](https://github.com/pyenv/pyenv/issues/465) and then reinstalling pyenv with brew (leaving all my .zshrc configurations in place).

```
rm -rf "$HOME/.pyenv"
brew uninstall pyenv
brew install pyenv
```

Once I was finally getting PIP working and able to cleaning re-install AWS CLI on my system I notice I had approximately 20 open tabs on Chrome that could almost trace my thinking and rabid searching.

Had I not found the solution and left it for later it wouldn't been doubtful I would have been able to pick back up from where I was.


## Development projects vs. learning

I currently have a project I've lost a bit of stream and enthusiasm for partly because of something similar. The project in question is a [parapos](https://github.com/paulywill/parapos) (this is a updated version of the original project I made many years ago:[Parachute-Packing-POS](https://github.com/paulywill/Parachute-Packing-POS)).

Since the skydiving season up here in Canada is soon to start and a fellow rigger friend was eager for me to help him create something I coded away, refactoring the original project and once again getting familiar with Rails. This included forcing myself to do a little [Freekend (free weekend) Hackathon](https://github.com/paulywill/freekend-hackathon-2018) to get most the functions working.

But trying to get this app deployed and production worthy has led me to installing some gems I've never heard of: [devise](https://github.com/plataformatec/devise) and [pundit](https://github.com/varvet/pundit). While it's rather easy to get the gist of what's happening and able to copy tutorials nicely, I'm lacking some serious knowledge gaps.

Thus a I looked into some TDD and RSpec (my local library provides us with free access to [Lynda courses](https://www.lynda.com) as part of their catalog) which then lead me to learning more subtle and essentials on the actual Ruby language and nothing related to Rails 5 (yet).


## Another Rerailment on Rails

I have a life coach. It's something I've been experimenting with a few months now. She's pretty amazing and always pointing out that we all have "saboteurs".

During our last session we went over my 5 strengths found from doing ["StrengthFinder Test"](https://www.gallupstrengthscenter.com/home/en-us/strengthsfinder). For US $19.99 I found out the [following](/assets/strengths.pdf) about me... I like to **Learn** and I like **Input**.  [wikipedia](https://en.wikipedia.org/wiki/Now,_Discover_Your_Strengths)

Thus, I have strengths for learning and taking in new information and probably some saboteurs for finishing projects and focusing.

The challenge she gave me after some discussion where I wanted to be professional was to register for AWS Development Certification.

To add the on the pressure I wanted to do it in [30 days](https://www.timeanddate.com/countdown/generic?iso=20180511T12&p0=1202&font=cursive).

Now my mind is jumping around once again. AWS training, Rails projects, and Ruby fundamentals.


## One thing

This is very ironic considering I just read [The ONE Thing](https://amzn.to/2IVjTDf) by Gary Keller and Jay Papasan.

If you can gather from the title, you focus and plan your life around ONE damn thing at a time, and setting up the dominos in your life.

In conclusion...

I'm now a little more calm and clear headed in this all night café and should probably head more to the worn down spouse.

After that, some more AWS training.

After that, finish and deploy my Rails app.

After that, level up my skills in Ruby and TDD with RSpec the next project down the road.

`saving`
`git push`
`closing tabs`
