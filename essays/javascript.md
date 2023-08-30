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
If an integer 0 equals a empty string and also equals a string "0" why does a string "0" not equal a empty array?

## Header

content here

## Header

content here

## Header

content here
