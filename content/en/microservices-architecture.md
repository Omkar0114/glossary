---
title: Microservices Architecture
status: Completed
tags: ["architecture", "fundamental", ""]
---

## What it is

A microservices architecture is an architectural approach that breaks applications into individual independent (micro)[services](/service/).
These services work together closely, appearing to the end user as a single entity. 
Take Netflix as an example. 
Its interface allows you to access, search, and preview videos. 
These capabilities are likely powered by smaller services that each handle one aspect, e.g., authentication, search, and running previews in your browser. 

This architectural approach allows developers to push out new features or update functionality much faster than if they were all tightly coupled, such as in a [monolithic application](/monolithic-apps/) (more to that below).

## Problem it addresses

Applications are made up of different parts, each responsible for a specific capability. 
Demand for a particular functionality will not necessarily increase or decrease with demand for other app parts. 
Going back to our Netflix example. 
Let's say that after a Black Friday discount campaign, Netflix experiences a big spike in signups, but streaming has remained more or less stable in the early hours of the day.  
The surge in signups demands more signup functionality capacity. 
Traditionally (monolithic approach), the entire app would have to be scaled to accommodate the signup increase — a very inefficient use of resources. 

Monolithic architectures also make it easy for developers to succumb to design pitfalls. 
Because all the code is in one place, it is easier to make that code [tightly coupled](/tightly-coupled-architectures/) and harder to enforce the principle of separation of concerns. 
Monoliths also often require developers to understand the entire codebase before deploying any chances. 
Microservices architecture is a response to these challenges.  


## How it helps

Separating functionality into different microservices makes them easier to deploy, update, and scale independently. 
By allowing different teams to focus on their own small part of a bigger application 
you also make it easier for them to work on their apps without negatively impacting the rest of the organization.
While microservices solve many problems, they also create operational overhead 
— the things you need to deploy and keep track of increase by order of magnitude or more. 
Many [cloud-native technologies](/cloud-native-tech/) aim to make microservices easier to deploy and manage.