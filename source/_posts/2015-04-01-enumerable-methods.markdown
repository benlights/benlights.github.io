---
layout: post
title: "Enumerable Methods"
date: 2015-04-01 21:27:12 -0400
comments: true
categories: 
---
#### Week Four Technical Blog Post

##### February 28, 2015

### Let's Get Profiling



In Ruby there are many ways of getting the same things done. In one example you can write extremely lengthy code or you can use an Enumerator. An Enumerator is a method that takes a block of code and runs a collection of data on piece at a time through it. Today I will be writing about the Enumerator`group_by`.

group_by is used to break a collection into "groups" based on the criteria that you give it. When it is called on a collection of data, it can be a hash or an array (of strings or integers), it runs on each piece and groups them by some criteria that I give it. Then it returns a hash with the key representing the group and the value an array of the "members" of that group.

Here is some code that will show you how it works.

![](/images/group_by-length.png)

In this example x was set to an array holding some strings, group_by was called to separate the strings by their length. The output was a hash`5 =>["hello"] 3=>["how", "are", "you"]` it grouped the strings the word "hello" has five letters as the key shows us, and the others all had three letters and are grouped together under the "3" key.

Another code example.

![](/images/group_by-modulus.png)

In this code snippet we ran the range 1 through 20 (that's what (1..20) means) and separated them by the remainders of four. They are grouped by what the remainder would be if the number was divided by four.

This is a very useful tool to have when you are trying to separate items.