---
layout: essay
type: essay
title: "Strict vs loose typing"
# All dates must be YYYY-MM-DD format!
date: 2023-08-29
published: true
labels:
- Engineering
- Coding Styles
---

<img width="200" class="rounded float-start pe-4" src="../img/javascript/JavaScript-logo.png">

*Loose typing in javascript, one week of learning*

This week I learned the basics of JavaScript and have used it to solve several problems.  I have not used JavaScript before, my coding experience is with C, C++, and python.

## Strict vs loose coding

I am experienced in strictly typed languages like C and C++.  Python is not a strictly typed language, it is however a strongly typed, dynamic language.  This means it is possible to change a variables type, for example from an integer to a string, however it does not do so in an unexpected way.  JavaScript is a loosely typed dynamic language, meaning it can dynamically change a variables type, but may do so in unexpected ways.  For example:
```
console.log(0 == []);       // Outputs true
console.log(0 == "0");      // Outputs true
console.log("0" == []);     // Outputs false
```
If an integer 0 equals an empty string and also equals a string "0" why does a string "0" not equal an empty array?  For another example, watch what happens when an integer is added to a string, then when the same integer and string are subtracted.
```
console.log(2 + "2");       // Outputs string "22"
console.log(2 - "2");       // Outputs integer 0
```
For the last example the code below outputs true:
```
console.log(0 == "0");  // integer 0 equals string zero, outputs true
console.log(0 == []);   // integer 0 equals empty array, outputs true
```
An integer 0 equals string "0", and integer 0 equals’ empty string.  It logically follows that string "0" should equal an empty string, since they both are equivalent to the integer 0.  This is not the case.
```
console.log("0" == []); // outputs false
```
This kind of loose conversion between datatypes can cause all sorts of problems when debugging code and is why I prefer when there is a stricter typing in place to protect against these errors.

### Compiled vs Interpreted/Just In Time

C and C++ are compiled languages that need to be created for the specific hardware and operating system they are put on.  JavaScript is an Interpreted/Just in time compiled language.  Interpreted means that the code is red line by line into a program that interprets the code, and then runs it.  This has performance impacts and can slow down code.  Just in time compilation is when code is compiled to machine code as it is being run.  This increases the performance of the code compared to just interpreting the code.  The big advantage of Interpreting/Just in time compilation is that code can be easily shared between different CPU architectures and operating systems.

### My thoughts

Having used JavaScript just for one week I can’t say I hate the language, though the loose typing feels wrong on some level.  I look forward to learning about the nonblocking event loop that is supposed to make multithreading coding easier.
