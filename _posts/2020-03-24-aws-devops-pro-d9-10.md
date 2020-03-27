---
layout: post
title: AWS DevOps Professional Journey - Day 9-10
date: 2020-03-26 16:00:00 Z
permalink: "/aws-devops-pro-day9-10/"
categories: [aws]
tags: [devops-pro]
comments: true
# other options
---

COVID-19 continues to distract and suck the oxygen from just everything these days.

WFH is next to nil, as there's a full on change freeze and lack of communication from management and team leaders.

Meh. Study on. Also reading the `Unicorn Project` finally. I forget some of the principles and ploy from `Phoenix Project`, was a few years ago.

### TIL
- CodePipeline: yesterday and today learned/refreshed with two labs. Some of the provided lab code for the `buildspec.yml` was missing two vital parms.

```
artifacts:
  files:
    - '**/*'
  name: my-webapp-artifacts
```

- Adding more instances and a DeploymentGroup for prod EC2 instances (this month will probably be expensive)

- Adding some stages and group actions to my pipeline, this is certainly makes sense to me using TravisCI and Heroku in the past




