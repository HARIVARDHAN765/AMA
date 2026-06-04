# JavaScript Interview Questions & Answers

## 1. Adhikya Edammala: What is a variable?

A variable is a container used to store data values in a program. In JavaScript, variables can be declared using `var`, `let`, or `const`.

Example:
```js
let name = "Hari";
```

---

## 2. Allanki VV Manikanta Sai: What are data types in JavaScript?

JavaScript data types are:

### Primitive Data Types
- String
- Number
- Boolean
- Undefined
- Null
- BigInt
- Symbol

### Non-Primitive Data Types
- Object
- Array
- Function

Example:
```js
let age = 23;        // Number
let name = "Hari";   // String
let isStudent = true; // Boolean
```

---

## 3. Arpit Yadav: What is the scope of `let`, `var`, and `const`?

| Keyword | Scope | Can Reassign? | Can Redeclare? |
|----------|--------|--------------|---------------|
| var | Function Scope | Yes | Yes |
| let | Block Scope | Yes | No |
| const | Block Scope | No | No |

Example:
```js
{
  let a = 10;
  const b = 20;
}
```

`a` and `b` cannot be accessed outside the block.

---

## 4. Boorle Sowmya Sri Lakshmi: What are labels in JavaScript?

Labels are identifiers used with loops to control flow using `break` or `continue`.

Example:
```js
outerLoop:
for(let i = 0; i < 3; i++) {
  for(let j = 0; j < 3; j++) {
    break outerLoop;
  }
}
```

---

## 5. Kamparapu Lakshman: What is npm?

npm (Node Package Manager) is the default package manager for Node.js. It is used to install, manage, and share JavaScript packages.

Example:
```bash
npm install react
```

---

## 6. Md Musharaf: Types of export in JavaScript

### Named Export
```js
export const name = "Hari";
```

### Default Export
```js
export default function greet() {
  console.log("Hello");
}
```

Importing:
```js
import greet from "./file.js";
import { name } from "./file.js";
```

---

## 7. Naman Sharma: How to select an HTML element using JavaScript?

Methods:

```js
document.getElementById("id");
document.getElementsByClassName("class");
document.getElementsByTagName("p");
document.querySelector(".class");
document.querySelectorAll("p");
```

Example:
```js
const heading = document.getElementById("title");
```

---

## 8. Nayunipatruni Harsha Vardhan: What is a JavaScript object?

An object is a collection of key-value pairs used to store related data.

Example:
```js
const person = {
  name: "Hari",
  age: 25
};

console.log(person.name);
```

---

## 9. Parlapalli Sulochana: How to run a JavaScript file in the terminal?

1. Install Node.js.
2. Open terminal.
3. Navigate to the file location.
4. Run:

```bash
node filename.js
```

Example:
```bash
node app.js
```

---

## 10. Rongala Vasu: Types of operators in JavaScript

### Arithmetic Operators
```js
+ - * / %
```

### Comparison Operators
```js
== === != !== > < >= <=
```

### Logical Operators
```js
&& || !
```

### Assignment Operators
```js
= += -= *= /=
```

### Ternary Operator
```js
condition ? value1 : value2
```

---

## 11. Rovinpal Udupi: What are Higher-Order Functions?

A higher-order function is a function that takes another function as an argument or returns a function.

Example:
```js
const numbers = [1, 2, 3];

numbers.map(num => num * 2);
```

`map()` is a higher-order function.

---

## 12. Tumma Haritha: What is `undefined` in JavaScript?

`undefined` means a variable has been declared but has not been assigned a value.

Example:
```js
let x;
console.log(x); // undefined
```

---

## 13. Vikas Mehta: What is lexical scoping?

Lexical scoping means a function can access variables from its outer scope based on where the function is defined.

Example:
```js
function outer() {
  let name = "Hari";

  function inner() {
    console.log(name);
  }

  inner();
}

outer();
```

Output:
```
Hari
```

---

## 14. Yash Nitin Raut: Can we declare private variables in JavaScript?

Yes. Modern JavaScript supports private class fields using `#`.

Example:
```js
class Person {
  #age = 23;

  getAge() {
    return this.#age;
  }
}

const p = new Person();
console.log(p.getAge());
```

Private variables cannot be accessed directly outside the class.

Example:
```js
console.log(p.#age); // Error
```

---