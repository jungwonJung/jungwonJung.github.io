---
title: JavaScript - An Interpreted, Dynamic, Object-Oriented Language with Primitive Types
author: JungWon
date: 2023-08-04 17:50:00 +0200
categories: [JavaScript]
tags: [typography]
pin: true
math: true
mermaid: true
---

# 1.Introduction to JavaScript

JavaScript is an interpreted language, which means it can be executed directly without the need for a compilation process like in compiled languages such as Python. Additionally, it is a dynamic language, which means that it allows for dynamic typing. This allows developers to change the data type of a variable on-the-fly, as demonstrated in the following code block:

```javascript
let x = 1;
x = "hello";
x = true;
x = { a: 1, b: 2 };
x = [1, 2, 3, 4, 5];
x = function (a, b) {
  return a + b;
};
```

# 2.Object-Oriented Concepts in JavaScript

JavaScript is also an object-oriented language, but its implementation of object-oriented concepts differs from languages like C++ and Java. JavaScript is based on prototypes and uses a first-class object model that allows for functional programming.

# 3.Primitive Data Types in JavaScript

JavaScript has primitive data types, which are simple data types that hold a single value. One of these primitive types is symbol.
It’s worth noting that JavaScript does not differentiate between integers and floating-point numbers;
both are considered number types. Additionally, undefined and null are both considered values in JavaScript.
In cases where a variable is assigned no value or is unknown, JavaScript stores this value in the data area as undefined.
null is typically used when an object should be present, but for some reason, it isn’t or when an object creation fails.

# 4.Quirks in JavaScript

One interesting quirk in JavaScript is that typeof null returns object. This is due to an error that occurred during the language’s initial design. While null is a value, it’s not an object, which can lead to confusion. Objects are not primitive types in JavaScript.
