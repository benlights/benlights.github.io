---
layout: post
title: "Chutes and Ladders or D&amp;D?"
date: 2015-04-01 21:28:47 -0400
comments: true
categories: 
---
#### Week Five Technical Blog Post

##### March 8, 2015

### Classes and How To Use Them.



This is an example of a class.

![](/images/class-die.png)

This class creates a die that can be used to play various games. Let us break up the code step by step.

The first step is to call the "Class" method, we do that by writing "class" and then the name we want to give it.(In this case Die. (Classes start with capital letters.)) Now it is time to call the attributes. An "attribute" is a method built in to the class "class", in this case "reader" lets us read the amount of side the die has after we create it. Here we get to the methods the live in the Die class. The method "initialize" is used when creating most classes and it is what we use to set the amount of sides and what we want written on them. The next bit of code makes sure that we create a die with a minimum of one side.

Now comes the fun part do you see "@label" and "@sides"? They are what is called an instance variable, this means they can be used by any method that is contained in the class. All instance variables start with an "@" and they follow the same naming conventions that normal variables have.

After this we have a new method, a method that is contained in a class is called a instance method. This means it can only be called on an object of of the Die class. In our method "roll" we roll the die and it gives us one of the sides that we initialized the die with.

This class is very useful it can be used for a simple game of Chutes and Ladders or a complicated many sided die used in D&D. Because we have created this class we can do whatever we want with it. We can give it as many sides as we want, we can put what ever we want on them. With a little tinkering we can even make it return more than one side every time we call "roll" on the die.

So what are you waiting for go and have fun!