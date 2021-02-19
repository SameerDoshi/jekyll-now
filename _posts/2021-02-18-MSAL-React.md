---
layout: post
title: MSAL with React
---

# Protecting your internal apps
Buisness units often need to rapidly deploy internal applications- but how do you protect these apps?
Traditional approachs were to use an SSO provider or app based authorization.  The former required integraition with an SSO provider and could take weeks, the later is a big no-no: DO NOT WRITE YOUR OWN login providers!

You can quickly [add authentication by using App Service Authentication](https://docs.microsoft.com/en-us/azure/app-service/overview-authentication-authorization) on your app. For server-side apps in Java, C#, PHP, or JavaScript you could can access logged in users' attributes by looking at request parameters.  But what if your code is run client side in REACT?

The Microsoft Authentication Library (MSAL) can help.

# MSAL Sample App
[This sample app](https://github.com/SameerDoshi/react-msal-example) will require login, and when logged in will display the "Welcome <first name> <last name>.

To get it up and running:
1. Create a new app registration in Azure
2. Modify app.js with that client ID 
3. Modify app.js with the tenant ID 
4. run npm install
5. run npm start

# How to use the sample
The sample is a starter kit- you can and should modify it.  Hope this helps and if it does drop a comment on the github!
     
