---
layout: post
title: Azure DevOps Setup
---

## [Azure DevOps](http://dev.azure.com) is a PaaS Azure service that's virtually free for many people (ex: if you're using Visual Studio it's probably free for you).
It's an awesome service that will quickly create a formalized SDLC to let you track work, automate (CI and CD!) all with no server setup.  Here's a quick video introdution:
[![Alt text](https://img.youtube.com/vi/JhqpF-5E10I/0.jpg)](https://www.youtube.com/watch?v=JhqpF-5E10I)

Let's use Azure DevOps to move faster and replace a need for Jenkins.  Jenkins is greate esp now that it's containerized and with annoucnement of a clud ative rewrite.  But we want to go full paas and never mange any infrastructure.
Azure DevOps is based on Team Foundation Server.

## GREAT! Let's Get Started
While it is easy to get started if you're familiar with TFS, it's daunting if you're more familiar with a traditional JIRA, git, jenkins stack.
Over the course of the next few posts let's get it setup in small, easy to digest chunks that you can manage between meetings.  

## Sample project
My project already has a matrue repo ,and I've been maintaing my backlog in a system I don't want to import.
My project is single user.  

## Goals
* source will remain in github
* Kanban board
* Move CI off my local dev
* Trunk based dev
* CD

