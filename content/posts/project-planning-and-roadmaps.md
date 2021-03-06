---
date: 2021-04-03T09:03:37Z
hero_image: "/content/images/alexander-schimmeck-io2zwcve8ci-unsplash.jpg"
tags:
- projectmanagement
author: Robert-Jan Korteschiel
title: Project planning and roadmaps

---
# Introduction

Currently, I am doing a project in which I have "accidentally" been tasked with planning out the features. I find this quite hard to do, and I'm not sure what the right way is if there is such a thing at all. It seems like a good topic to think about, so let's explore it a bit out loud.

When someone pitches a project or feature to you, I am often asked to write a quote or budget in some form. Often that is a simple email, but when the project is larger than the average marketing site, I might plan it a bit more rigorously. So I use a Trello template, I set up a more user-focused Productboard, or I might even try to do it the "right" way by starting up a full-blown Jira workspace. I plan out what I think needs to be done and end up with a really long and messy list. Once there, it becomes clear that it needs to be structured somehow, so I start asking myself questions like "who is my audience?" or "what perspective should I use?". I soon realize that this is taking a lot of time, and almost every time, I decided to wing it. Just building the thing is easier, especially when working alone. I will hit the next thing on the list in a very intuitive way without planning at all. Once I start working, I know I will finish the project at a certain point. So when writing the quote, I put my finger in the air and jot down an almost random number. I use wonderful time logging software, so I will know exactly how far I was off.

On the other hand, I have the things that I am learning in my study in information sciences and the other stuff that I experienced and read. I have often heard about the big methodologies for organizing projects, like the dichotomy between waterfall and agile methodologies. Neither seems really attractive. The "big design up front" waterfall methodology seems always to yield unhappiness because it tries to control the unknown upfront. You do not know what you will encounter before you encounter it. The agile methodology is not much better. It always ends with the wonderful anecdote "let's design in code," which is short for letting the developer spend time on product management and UI / UX design in an incredibly inefficient tool for that job. Both large methodologies seem terrible in their extremes, yet the concepts gnaw at you. You don't want to waste time planning, nor do you want to waste time building something nobody will appreciate. The much-discussed reason technological initiatives fail is the gap between business needs and technological implementation. You also know that deploying a theory in a practical context is often the best way to make a messy situation worse. 

So I am locked between the practical time hog of planning and the academic "it depends on the context." So how to break this up a bit better?

## What and how am I planning?

![](/content/images/microsoftteams-image.png)

So yesterday, I made another attempt at managing a product in a structured fashion, and lo and behold, the messy long list of a thousand entities was back again. This time I was using Productboard to produce a set of features for the project I was working on. But after a few hours of playing around, I couldn't make something good, which was confirmed by feedback on what I had been doing. I already felt that it was too specific, and someone who viewed it felt it was "top-heavy" as well. So in the evening, I started to abstract from the things I had been doing during the day and created this whiteboard, vaguely remembering some methodologies I've read about at one point. It shows three levels, the organization level with stakeholders and processes and the system level with front-end and back-end (which ended up being largely the same).

![](/content/images/img_0975.jpeg)

What became clear is that I was messing around with multiple entities:

* **Requirements:** Quite general things like security or usability
* **Processes:** content strategy, marketing, design workflows, CI/CD, technology and user monitoring & analytics, etc.
* **Features:** Things that the user would really like to have or we would like to build for some reason.
* **Issues:** Things that a causing us or users problems, like bugs and reported UI / UX problems, often things that look small but might be deceptively complicated.
* **Tasks or sub-features:** Smaller entities to break up the complexity of the larger entities.

I also wanted to apply them against time, so I started using:

* **Timeframes:** Basically a start and end date for an entity
* **Releases:** Groupings of entities within a timeframe to create packages of features that deliver a certain value

Note that this was already an improvement, I tried to do this a few times before, and sometimes I even went down to a technological level in planning by using things like:

* **Applications or services:** The largest entities within a system
* **Components, modules, or views:** Large entities by which you break up a system
* **Interfaces:** The boundaries between components
* **Actions or events:** The things that can happen within the system
* **Functions or objects:** The atomic bits of the application

Apparently, I am still dealing with the abstraction level I should use to think about these things. Each of these entities describes an important thing, yet when to use which is the question. I brought my own knowledge as a developer, and I brought my knowledge as an information scientist together. In the meanwhile, I was engaging with the data model that Productboard was pushing onto me. But all of these different views actually didn't make things easier, and I actually had to reconcile them into a good mental model for myself first. Perhaps because I don't understand the boundaries between all of these concepts, or perhaps because this is always very hard to do well. In truth, it doesn't matter what my level of knowledge is, the job still needs to be done, or else we're back to"let's see what happens" and "let's go plan & design & test with the actual code." That will grind the process to a halt and feel like a defeat.

# What to do about it?

So the question arises, what to do about it? I think I will go back to the reason I chose Productboard in the first place: I wanted to be constrained by the data model, methodology, and functionality that they provide. Hopefully, they have thought about the problem a lot more than I have. My goals seem to align, and I am not writing to plan out the project but research and validate features when they are still just plain text (and maybe a quick sketch). In the project we are currently working on, we need to test many features and ideas in low-fidelity. We are starting to do some research and attempting to structure it, but we're not yet testing cheaply. This reaffirmed my original goal; I wanted to write out ten features to validate them. 

I got lost because I did not consider what a feature truly was. The level of abstraction I needed to think was not yet clear to me. After writing this out, I think I can accept at which level a feature lies. I think it is not quite as abstract as a general requirement like "security."  On the other hand, is it quite big, making thinking at a technological level irrelevant, you probably need to do things at every level. For now, I will resist placing the features on a timeline and revert to a now, next, later strategy. I cannot predict those timelines accurately anyways. That insight needs to grow organically. I do not think it actually matters that much. Things will go as fast as we can make them go. We have to find another way to measure whether we are doing good work. A continuous stream of delivered value or an upbeat in sales is probably a better measurement than the comfy feeling of pride that we estimated the time it took to build features properly. 

As for how I will write them, I also remembered something about user stories I read a while back. A user story is written like this, according to Wikipedia: 

> As a -_role-_ I can -_capability-_, so that -_receive benefit-_

While I was not too fond of the formatting of the various way of writing them, which I feel removes all the creativity from the process, I do like the concerns they address. I want to present a feature with a certain role and task in mind, which we can solve to deliver value. I also want to describe the context, a time, and a place of the feature to situate it a bit. 