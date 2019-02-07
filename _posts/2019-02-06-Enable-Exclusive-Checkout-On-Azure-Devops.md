---
layout: post
title: Enable Exclusive Checkout on Azure DevOps 
---

# What is Exclusive Check Out
If you've ever used ClearCase, pCVS, or TFS you may have used a workflow in which you check-out a file while you edit it.  When you're done with the file you check it in and others are free to check it out in order to edit it.
The key idea: *ONLY* one person can edit a file at once.

# But Why?
If you're using git, you might wonder why someone would use a workflow like the one above. If you're dealing with binary files, static content, or other assets that can't be _diffed_.

# Enabling Exclusive Check out in Azure DevOps

## Set Azure DevOps project to use a TVCF Repository

You'll need to add a TVCF Reoi
(Screen shots pending)

## Set Visual Studio
### Setup Workspace
    * Manage Workspace
    * Select active workspace, click edit
    * Click Advanced
    * Ensure Location is set to Server
    * Verify Server is set to dev.azure.com/<org>

### Setup Team Explorer
    * (under team explorer) clicked "Settings"
    * (under "Team Project ")  click "Source Control" change type to “server” click ok
    * (under “Team Project”) click “Source Control”  then uncheck "multiple check-out"
