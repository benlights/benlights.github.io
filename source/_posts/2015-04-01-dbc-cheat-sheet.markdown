---
layout: post
title: "DBC Cheat Sheet"
date: 2015-04-01 21:19:02 -0400
comments: true
categories: 
---

### Ruby Hashes, Arrays, Strings, Integers

#### Hashes

If you attempt to access a hash with a key that does not exist, the method will return nil.

You can create an empty hash with the new class method:`months = Hash.new`  

You can also use new to create a hash with a default value, which is otherwise just nil:`months = Hash.new( "month" )`or`months = Hash.new "month"`

You can use any Ruby object as a key or value, even an array, so following example is a valid
`[1,"jan"] => "January"`  

##### A list of useful methods.

`hash.delete_if { |key,value| block }`
Deletes a key-value pair from hash for every pair the block evaluates to true.

`hash.each { |key,value| block }`
Iterates over hash, calling the block once for each key, passing the key-value as a two-element array.

`hash.each_key { |key| block }`Iterates over hash, calling the block once for each key, passing key as a parameter.

`hash.each_key { |key_value_array| block }`Iterates over hash, calling the block once for each key, passing the key and value as parameters. 

`hash.each_key { |value| block }`Iterates over hash, calling the block once for each key, passing value as a parameter.

`hash.empty?`Tests whether hash is empty (contains no key-value pairs), returning true or false.

#### Arrays

Creating Arrays:  
One way is with the new class method:`names = Array.new`  
You can set the size of an array at the time of creating array:`names = Array.new(20)`  
here is another method of Array, []. It works like this:`nums = Array.[](1, 2, 3, 4,5)`  
One more form of array creation is as follows :`nums = Array[1, 2, 3, 4,5]`  

##### A list of useful methods.

`array.clear`Removes all elements from array.

`array.collect { |item| block } [or]``array.map { |item| block }`Invokes block once for each element of self. Creates a new array containing the values returned by the block.

`array.collect! { |item| block } [or] array.map! { |item| block }`Invokes block once for each element of self, replacing the element with the value returned by block.

`array.delete_if { |item| block }`Deletes every element of self for which block evaluates to true.

`array.each { |item| block }`Calls block once for each element in self, passing that element as a parameter.

`array.each_index { |index| block }`Same as Array#each, but passes the index of the element instead of the element itself. array.empty? Returns true if the self array contains no elements.

`array.eql?(other)`Returns true if array and other are the same object, or are both arrays with the same content.


#### Strings

##### A list of useful methods.

`str * integer`Returns a new string containing integer times str. In other words, str is repeated integer imes.

`str.capitalize`Capitalizes a string.

`str.casecmp`Makes a case-insensitive comparison of strings.

`str.chop`Removes the last character in str.

`str.downcase`Returns a copy of str with all uppercase letters replaced with lowercase.

`str.include? other_str [or] str.include? fixnum`Returns true if str contains the given string or character.
`str.reverse`Returns a new string with the characters from str in reverse order.

`str.split(pattern=$;, [limit])`Divides str into substrings based on a delimiter, returning an array of these substrings. If pattern is a String, then its contents are used as the delimiter when splitting str. If pattern is a single space, str is split on whitespace, with leading whitespace and runs of contiguous whitespace characters ignored.

`str.swapcase`Returns a copy of str with uppercase alphabetic characters converted to lowercase and lowercase characters converted to uppercase.

#### Integers

##### A list of useful methods.

`next → integer` Returns the Integer equal to int + 1, same as #next.

`pred → integer`Returns the Integer equal to int 

`odd? → true or false`Returns true if int is an odd number.

`Round([ndigits]) → integer or float `Rounds int to a given precision in decimal digits (default 0 digits). Precision may be negative. Returns a floating point number when ndigits is positive, self for zero, and round down for negative.

`chr([encoding]) → string `Returns a string containing the character represented by the int‘s value according to encoding.	