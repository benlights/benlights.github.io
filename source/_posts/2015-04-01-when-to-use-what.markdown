---
layout: post
title: "When to use what"
date: 2015-04-01 21:30:24 -0400
comments: true
categories: 
---
####Week Six Technical Blog Post

##### March 15, 2015

### Variable Scope



Today I will be writing about variable scope. Scope defines where in a program a given variable is accessible. Ruby has four types of variables each can be accessed by different parts of a program hence "scope". The four types are: local, instance, class and global.

The first type, Local Variables are local to the method or code they are declared in. Naming convention also states that they start either with an underscore `_` or a lower case letter. If you try to use a local variable in a method that it was not declared in it will give you an error: `"NameError: undefined local variable or method ``x' for main:Object"` This is because outside of the local method in which the variable was declared it does not exist.

The next type is the Instance Variable. This variable is available to any instance of a class. If I have a class `Bike` with an instance variable `@gears` and I instantiate a new instance of Bike, let's call it `mountain_bike`, `@gears` -the one that belongs to `mountain_bike` will only be accessible to `mountain_bike` not to any other instance of the class Bike. Instance Variables start with an `@`.

Class variables are similar to instance variables but it is shared across all instances of the class. Going on the earlier example `@@gear` will now be accessible not just to mountain_bike but to any instance of Bike. Class variables start with `@@`.

Global variables start with an `$` and are discouraged from use. This is because they can be read and changed from anywhere in the code and this makes it very hard to track down bugs. They are accessible to any and every bit of code.