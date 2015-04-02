---
layout: post
title: "Arrays Vs. Hashes"
date: 2015-04-01 21:25:45 -0400
comments: true
categories: 
---
#### Week Three Technical Blog Post

##### February 22, 2015

### Showdown: Arrays vs. Hashes


This week we have started learning Ruby. Ruby is a high level object-oriented language. There is much to explore in Ruby and I have going at it all week, but in this blog post I want to talk about two objects in Ruby that have helped enormously in completing my exercises for the week.

Arrays and Hashes. Arrays and Hashes are both ways of storing information that is assigned a label in Ruby. However they are not the same and each have their own uses.

Array: An array is list of information that is tied to its order in numbers. This list can be made up of "strings"(regular text), integers, floats(numbers with decimal points) and even other arrays. The way to initialize an array is to put a set of elments between square brackets like this:

`a = [ 1, 'cat', 3.14 ]`   An array with three elements 

Each element in the array is set to a specific number. 1 is set to 0 (arrays always start from zero) "cat" is 1 etc. 

Now that they are set in the array they can be called and have methods work on them.

Hashes: Hashes are similar to arrays but you need to supply both the key and the value. For example if you want 1 to equal "cat" you would have to set it. Hashes are initialized with squiggly brackets like this:

    my_hash = {
      1 => 'cat'
      }
if I would want to call cat I would have to write 1\. But with a hash I can set it to be anything I want.    
`my_hash = {
      'kitten' => 'cat'
      }`

Now I have to call 'kitten' to get back cat.