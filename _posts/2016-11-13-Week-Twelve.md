---
layout: post
title: "Week Twelve: Abstraction"
---

### What did I do this past week
This week we looked more at subclassing and how to create an abstract class. Unlike in other languages where you can define an interface or protocol that a class can then conform to, C++ simply has classes. This means that the abstract class that you create must have its own implementation of its methods, and since it really is just a class, you can create instances of it. With looking at inheritance, we also looked at how you can view subclasses as their parent class, but without the extra information the child class defined. Unfortunately, the only way to look at a class as if it is its parent class without actually losing its more specific information is by using pointers. This leads to more issues such as having a vector of an abstract class, because in order for those abstract classes to correctly be the child classes, it must be a vector of pointers. Since we are now working with pointers instead of objects, we run into a bunch of new issues. The solution is that when creating an abstract class, you also create a container class for that abstraction that simply holds a pointer to the abstract class so that it can handle all of the things it needs to, and then the container can simply be treated as the abstraction if you want to use multiple types of that abstraction.

### What's in my way
Generally classes are starting to wrap up their projects and tests for the semester, so I am making sure I have all my assignments done, and content studied. Other than that I just need to keep my school work balanced with actual work.

### What will I do next week
This week I am finishing up two essays, two units for an online class, and completing the life program for this class.

### My experience
Generally learning about how to make abstractions in C++ has been pretty interesting. However, I tend to prefer the protocol way of creating abstractions, such as in Swift and Objective-C. Having to create both an abstract class that acts as the parent class, and a container class to be used when working with multiple versions of the abstraction seems fairly messy. Both the container and the abstract class must have the same methods and values, since you should be able to use the container interchangeably with child classes of the abstraction, however since the container class holds a pointer to an instance of the abstract class, it doesn't actually subclass the abstraction. This means you need to have two matching interfaces, but they aren't actually connected in code, which seems unsafe. Having to implement the methods of the abstract class and being able to create an instance of the class also seems messy and unsafe. Furthermore, since you should be able to use the container and the child classes in the same way, there doesn't really seem to be a good way to use public variables without having getters and setters for all the classes.

### Tip of the week
Today's tip of the week: Plan out your code before actually programming anything. This could be done in many ways such as drawing out diagrams or writing sudo code. Having a plan before jumping right into a solution will help keep your code cleaner, and will help you get the problem right sooner.
