---
layout: essay
type: essay
title: "Reflection on Javascript"
# All dates must be YYYY-MM-DD format!
date: 2023-08-29
published: true
labels:
- Engineering
---

<img width="1052" class="rounded float-start pe-4" src="../img/javascript/JavaScript-logo.png">

*Reflection on javascript after one week of learning.*

This week I learned the basics of javascript and have used it to solve several problems.  I have not used javascript before, my coding experience is with C, C++ and python.

## Strict vs loose coding

I am experienced in strictly typed languages like C and C++.  Python is not a strictly typed language, it is however a strongly typed, dynamic language.  This means it is possible to change a variables type, for example from a integer to a string, however it does not do so in an unexpected way.  Javascript is a loosely typed dynamic language, meaning it can dynamically change a variables type, but may do so in unexpected ways.  For example:
```
console.log(0 == []);       // Outputs true
console.log(0 == "0");      // Outputs true
console.log("0" == []);     // Outputs false
```
If an integer 0 equals a empty string and also equals a string "0" why does a string "0" not equal a empty array?  For another example watch what happens when a integer is added to a string, then when the same integer and string are subtracted.
```
console.log(2 + "2");       // Outputs string "22"
console.log(2 - "2");       // Outputs integer 0
```
This kind of loose conversion between datatypes can cause all sorts of problems when debugging code, and is why I prefer when there is a stricter typing inplace to protect against these errors.

## Compiled vs Interpreted/Just In Time

C and C++ are complied languages that need to be created for the specific hardware and operating system they are put on.  Javascript is an Interpreted/Just in time compiled language.  Interpreted means that the code is red line by line into a program that interprets the code, and then runs it.  This has performance impacts and can slow down code.  Just in time compilation is when code is compiled to machine code as it is being run.  This increases the performance of the code compared to just interpreting the code.  The big advantage of Interpreting/Just in time compilation is that code can be easily shared between different CPU architectures and operating systems.

## My thoughts

Having used javascript just for one week I cant say I hate the language, though the loose typing feels wrong on some level.  I look forward to learning about the nonblocking event loop that is supposed to make multithreading coding easier.

