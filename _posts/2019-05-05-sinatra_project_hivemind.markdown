---
layout: post
title:      "Sinatra project: HiveMind"
date:       2019-05-05 04:51:16 +0000
permalink:  sinatra_project_hivemind
---


This project was very satisfying. What first started off as a simple CRUD application using Sinatra's MVC architecture turned into a great learning opportunity for Rails, Javascript, and much more. 

I approached this project with the mindset of using Sinatra as a base to build out more complex features that resemble some Rails functionality. I was inspired to do this after thinking of my old math classes, where we learned to calculate functions such as integrals using long-handed calculations that were sometimes grueling, but very instructive. This method made the transition to easier calculation methods much less "magical." 

An example of the functionality are the partials integrated into my project. While I don't know if my implementation was followed best practices, it did significantly reduce the complexity of my views, particularly similar forms I used to create/edit beekeepers and hives. I am also currently implementing Sinatra's version of strong params using an open source gem.

Another cool tidbit I picked up came in the form of many tutorials I ran into while researching the different things I was implementing, in the form of Haml. Haml stands for HTML abstraction markup language. Unlike erb, which just embeds ruby into already-existing html, haml provides a less verbose markup language that better incorporates ruby. It also provides better structuring while following coding principles like DRY.

As an example, take the following erb:
```
<div class="container"
  <h1>
    <%= @foo.name %>
  </h1>
</div>
```

can be written much cleaner in haml as:
```
.container
  %h1 #{@foo.name}
```

While the learning was a lot to take in up front, I found the amount of time I was coding views went down significantly after getting the hang of it.

One of the biggest struggles I had was coding all the styles from scratch. However, the experience has really built up my foundational understanding of css, and I look forward to using some cool frameworks in the future to really step up my layouts. I will say that I have a lot to learn when it comes to designing a UI that I can really be proud of, but a goal of mine is to reach out to people I know to get help with the UI/UX aspects of my project and in general.

Other things I built into my project: javascript event listeners, securing session secrets, model validations

What I still want to incorporate: blog posts, hive entries, post comments, a search function for beekeeper associations.

This project was a great learning experience, but time dictates I move onward and upward! I sincerely hope I can come back to this project, however.

