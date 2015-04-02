---
layout: post
title: "SQL Injection"
date: 2015-04-01 21:36:19 -0400
comments: true
categories: 
---
####Week Eight Technical Blog Post

##### March 28, 2015

### Little Bobby Tables



Today I will be writing about SQL Injection. SQL Injection is a way to insert code maliciously into an entry field in an application. This attack can be used against any database but is usually used against websites.

There are a few different methods that are used to maliciously send commands to the server. Today I will be writing about one of them.

Incorrectly filtered escape characters.

This type of SQL Injection occurs when input from user entry fields are not filtered for escape characters. Escape characters are special characters used in programming that tell the program, that the character after them is not to be read the usual way rather as a different character. A common example is the "\".

For example, an name entry field in a website. The website takes the input from the field and turns it into a select statement.

    `SELECT * from USERS WHERE name = (entry field);`

This code looks for the specified user name and returns it from the database. 

However this user name can be set to whatever the person on the other side of the field wants. 

For example if    `'' or '1'='1'` is entered it turns into the following SQL statement    `SELECT * FROM users WHERE name = '' OR '1'='1'`; 

This statement would return all the names in the database because`1 = 1` is always true.

This vulnerability can also be exploited to delete or modify data in the database. See the story of[ Little Bobby Tables.](https://xkcd.com/327/)