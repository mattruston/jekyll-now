---
layout: post
title: "Week Eleven: R values"
---

### What did I do this past week
The main focus of this week was looking at R values, using them to our advantage when optimizing our constructors and assignment operators. This becomes useful when you are initializing a variable or assigning a variable with the return value of a function. Typically, without optimization the value that is returned must be copied and then deleted. This is not the best since we are deleting a value that we really want to keep. The idea that comes in is moving that value instead of remaking it and letting the previous one die. C++ 11 introduced the double & identifier when declaring a variable. The && means that it is an R value, that is, a value without an address, or a value that is typically found on the right side of a statement. By using the && and the move function, we were able to create methods that only run when an R value is passed in. This way we know that the value doesn't actually live anywhere and we can just move its values to where we want them.

### What's in my way
This past week I have been sick, which has been unfortunate for trying to stay productive. My hope is that it will clear up soon, but if that is not the case, it will be in my way. The semester is also quickly coming to a close, so I need to make sure I get all my last projects that are coming up done.

### What will I do next week
This week I have a presentation for my architecture class, some essays for other classes, and I get to start working on our last program for this class. Similar to the last program, we are doing another simulation type program, this time simulating life.

### My experience
Learning about R values more and how we are able to distinguish them in C++ has been pretty interesting. Up until this class I had never even heard of R values and L values, so it is neat to have a name for the concept. The most odd thing to me is that you can declare a variable as an R value using the &&, but as soon as you do so, since it has a name, it isn't really an R value anymore. This is the case where you need to use the move function to let the complier know that this value should be treated as an R value.

### Tip of the week
Today's tip of the week: Make sure you get plenty of sleep. Being well rested allows your mind to stay sharp and you won't overlook simple problems in your code that normally wouldn’t take you any time at all.
