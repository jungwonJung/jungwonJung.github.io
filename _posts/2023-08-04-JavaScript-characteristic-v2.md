---
title: Characteristics of Compiled Languages and Numeric Data Types in JavaScript
author: JungWon
date: 2023-08-04 18:10:00 +0200
categories: [JavaScript]
tags: [typography]
pin: true
math: true
mermaid: true
---

# 1.Compiled Languages

- During compilation, data type errors are checked.
- JavaScript is not a compiled language, so it cannot check for data type errors during compilation.
- The lack of data type checking in JavaScript can lead to a high number of errors.
- The web does perform compilation to some extent, but errors can still occur during runtime.

# 2.Assignment Operator

- The += assignment operator creates side effects that change the value of the variable.

```javascript
let str1 = "hellow";
str1 += " world";

console.log(str1); // hello world

let str2 = (str1 += "~~~");

console.log(str2); // hello world~~~
console.log(str1); // hello world~~~
```

# 3.Numeric Data Types

- JavaScript does not have separate data types for integers and floating-point numbers.
- The numeric data type in JavaScript uses double-precision floating-point format, which is different from the 32-bit float format used in other languages.
- Due to the use of floating-point numbers, some calculations in JavaScript can result in rounding errors.

```javascript
console.log(0.1 + 0.2 === 0.3); // false

console.log(0.1 * 10); // 1
console.log(0.1 + 0.1 + 0.1 + 0.1 + 0.1 + 0.1 + 0.1 + 0.1 + 0.1 + 0.1);
// 0.99999999999999999999
```

- Infinity is a special value in JavaScript that represents an overflow error. It can be positive or negative.

```javascript
let y = -1 / 0;
console.log(y, typeof y); // -Infinity 'number'

let x = 1 / 0;
console.log(x, typeof x); // Infinity 'number'
```

- NaN is another special value in JavaScript that represents an error value. Its type is also number.
- To check if a value is NaN, you can use isNaN() or Number.isNaN() methods.
- Libraries are available for precise numeric calculations in JavaScript.
