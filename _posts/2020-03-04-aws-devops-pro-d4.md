---
layout: post
title: AWS DevOps Professional Journey - Day 4
date: 2020-03-04 13:00:00 Z
permalink: "/aws-devops-pro-day4/"
categories: [aws]
tags: [devops-pro]
comments: true
# other options
---

Another study day in the books. 

I don't know if this is good habit, but I start by comparing industry salaries for the job I [have](https://www.payscale.com/research/CA/Job=Mainframe_Systems_Programmer/Salary) with the [one](https://www.payscale.com/research/US/Job=Senior_Development_Operations_(DevOps)_Engineer/Salary) I inspire towards before studying. 

Motivating? I don't know.

### TIL
Continuing with the [Udemy Course](https://www.udemy.com/course/aws-certified-devops-engineer-professional-hands-on/):

- AWS just recently introduced [masks](https://forums.aws.amazon.com/thread.jspa?threadID=314535) for secure strings in the CodeBuild log
- [Indentation](https://github.com/awsdocs/aws-codebuild-user-guide/issues/46) in the `buildspec.yml` is very important and actually broke one of my builds. In this case the `artifacts` is indented under `phases`.


##### WRONG INDENTATION:
```yaml
version: 0.2

phases: 
    install:
        runtime-versions:
            nodejs: 10
        commands:
            - printenv
            - echo "installing something"
    pre_build:
        commands: 
            - echo "we are in the pre build phase"
    build:
        commands:
            - echo "we are in the build block"
            - echo "we will run some tests"
            - grep -Fq "Congratulations" index.html
    post_build:
        commands:
            - echo "we are in the post build phase"
            
    artifacts:
      files:
        - '**/*'
      name: my-webapp-artifacts

```

```log
[Container] 2020/03/04 17:13:10 Waiting for agent ping
[Container] 2020/03/04 17:13:12 Waiting for DOWNLOAD_SOURCE
[Container] 2020/03/04 17:13:16 Phase is DOWNLOAD_SOURCE
[Container] 2020/03/04 17:13:17 CODEBUILD_SRC_DIR=/codebuild/output/src501708359/src/git-codecommit.ca-central-1.amazonaws.com/v1/repos/my-webpage
[Container] 2020/03/04 17:13:17 YAML location is /codebuild/output/src501708359/src/git-codecommit.ca-central-1.amazonaws.com/v1/repos/my-webpage/buildspec.yml
[Container] 2020/03/04 17:13:17 Phase complete: DOWNLOAD_SOURCE State: FAILED
[Container] 2020/03/04 17:13:17 Phase context status code: YAML_FILE_ERROR Message: Invalid buildspec phase name: artifacts. Expecting: build,install,post_build,pre_build

```



##### CORRECT INDENTATION:
```yaml
Edit
No lines are selected.
version: 0.2

phases: 
    install:
        runtime-versions:
            nodejs: 10
        commands:
            - printenv
            - echo "installing something"
    pre_build:
        commands: 
            - echo "we are in the pre build phase"
    build:
        commands:
            - echo "we are in the build block"
            - echo "we will run some tests"
            - grep -Fq "Congratulations" index.html
    post_build:
        commands:
            - echo "we are in the post build phase"
            
artifacts:
  files:
    - '**/*'
  name: my-webapp-artifacts
```



- [YAML](https://yaml.org/faq.html) - spaces wins this round tabs!