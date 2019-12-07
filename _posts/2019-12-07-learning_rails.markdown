---
layout: post
title:      "Learning Rails"
date:       2019-12-07 07:10:21 +0000
permalink:  learning_rails
---


Coming off of Sinatra, I was feeling pretty exhausted. I challenged myself to write out several parts of my project in haml instead of erb, for example. I also chose to write all of my css styles from scratch. Honestly, what was I thinking?

To be fair, though, the struggle of those challenges made me learn so much more. 

I was definitely glad to move onto Rails, however. The land of magic. Helpers for every case, conventions for every character typed. The ease I felt when progressing through Rails was nothing short of amazing. 

That didn't last long.

I found a way to make things harder for myself (again), and thus Motimates was born. Motimates is an app I was inspired to make from the concept of an accountability buddy, basically someone who holds you accountable to the expectations you have set for yourself. I derived the name from "motivation" and "mate" (as in friend). It takes the shape of a social networking site where you can add friends (ie motimates) that will help you stay true to certain goals you have added on the site.

While it sounds easy up front, this concept can actually pose many challenges within the Rails framework. How (in the database) can a user be related to another user (self-referential relationships)? How can we ensure the other side of said relationship is also accounted for (bi-directional)? How will these users find each other?

These were all questions I had to answer along the way. And boy was it a struggle.

I also challenged myself to incorporate several popular libraries within the Rails community. I used Devise and omniauth gems to provide basic authentication and google oauth, CanCanCan to allow for easy authorization checks in my controllers and views, and (more natively) ActiveStorage for image uploads.

It's been amazing because I'm finding reading documentation and picking up new technologies so much easier now. It has admittedly lead to me wanting to read documentation for everything under the sun that sounds interesting...which is basically everything! Turbolinks? Read it. Graphql? Read it. ActionCable? Well, tried to read it.

That leads to my second breakthrough with this project, which was really pinpointing my flaws in terms of staying focused on the task at hand. I've begun to get much better at breaking up projects into smaller tasks up front instead of as I go. I still have a tendency to get distracted by shiny new things, but it's getting better.

All in all, this project was really fun and has me motivated to incorporate javascript to make it even better.

Things I would like to improve on include:

-having a chat system

-having a more SPA feel, which could influence my layouts

-adding in multiple photos (profile pic + album of past photos)

-have comment system

Now onto javascript!
