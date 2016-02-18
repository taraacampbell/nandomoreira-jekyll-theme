---
layout: post
title: "Think Like A Programmer"
date: 2016-02-04 09:15:20
comments: true
description: ""
keywords: ""
categories:
- welcome
tags:
- welcome
---

Hashes and arrays are two ways of storing data, in bulk. However, the main difference in them is how specific each can get. To get a visual, arrays are like an office space, with each string or integer, etc. being a cubicle. We can go to each cubicle according to a person’s name, or whatever we’ve named a string in that array. A hash is like an office building floor, with each key being an office. Every office has cubicles, which are the subgroups of that key.

A buyer will choose either format depending on what kind of space they need. If it’s a smaller company with fewer employees, then a simple office space will do just fine, or in our case an array. If you want more space to put your larger company, you’d buy a floor, which is what we’re comparing to a hash, since they’d need more space for specific parts of the company.

Hashes can be used for storing things like music or movies, because there are layers to the information such as artist and album title, which the key (the song) can point to. Arrays can be used to display ice cream flavors, but a good example of a nested array within a hash is at a desert shop: keys can be categories such as ice cream, cookies, cake and then within those keys are arrays of the flavors or types of cookies available. We saw this in our chipotle array/hash practice, and I can imagine that it’s similar to the way computers store our orders in real life. If we want to order a cake, we would click on a cake then flavor and frosting. All the buttons we’re pressing come up as a result of the key being pressed, then the array following with the subgroups, or the options for cake flavors, etc. This is also similar to a phonebook example given in Dictionary.com’s definition of hash coding.

Depending on the complexity of data, and length of a program, a hash will most often be more comprehensive than arrays. If it’s too daunting to use a hash, multiple arrays can also do the trick, but in lengthier matter. It’s important to gauge the need for a hash, too; sometimes a hash is too much “filing” for a certain set of data. If it can be simplified, make sure it is! 

https://teamtreehouse.com/community/when-do-you-use-an-array-versus-a-hash-in-ruby
http://dictionary.reference.com/browse/hash-coding
http://stackoverflow.com/questions/6097637/whats-the-difference-between-arrays-and-hashes
