---
title: Incorrect Gmail password when using exchange on iPhone
author: Jacob Tomlinson
layout: post
permalink: /2012/09/12/incorrect-gmail-password-when-using-exchange-on-iphone/
category: iPhone
thumbnail: gmail
tags:
  - Gmail
  - Google
  - iPhone
  - Microsoft Exchange
---

### The Problem  
Recently I've tried playing around a little with the email account settings on my iPhone to try and get as much to sync as possible with some of my other accounts. One thing I did was to change Gmail from the standard 'Gmail' setting that you get on iOS to the 'Microsoft Exchange' setting as recommended by Google.

Among other things this allows my phone to sync contacts with my Gmail account without having to plug into a pc with iTunes. However when I set this up my phone kept intermittently telling me that my Gmail password was incorrect, so every time this came up I would put my password in and it would reject it. For a while I wasn't sure if I was just being silly and typing it incorrectly on the iPhone keyboard or if something has gone a bit wrong.

![Gmail Incorrect Login](http://i.imgur.com/1JAJSVX.png)

### The Solution  
After a little googling around I found a nice blog post, which has sadly now been taken down, by someone who had found the same problem. They found that this issue is due to Google having a captcha on the login page the Exchange was trying to log in with, this meant that each login it was failing the captcha and therefore the login. To remedy this I visited the <a title="Application specific passwords" href="http://support.google.com/accounts/bin/answer.py?hl=en&answer=185833&topic=1099586&ctx=topic" target="_blank">Google page for creating application specific passwords</a> and created one called 'Gmail on my iPhone'. Then went into the Gmail settings on my phone, put in the password that Google generated for me and it started working.

This works because when you login with an application specific password it skirts around any extra authentication like captchas or the 2-step authentication text messages as the passwords generated are single use and can only be generated by the user when logged in and authenticated. You also have the ability to revoke any app specific passwords which is nice because if you lose your phone or laptop or any device using one you can just revoke that specific password rather than having to change your password entirely.