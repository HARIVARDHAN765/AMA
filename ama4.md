# AMA

# 1. Difference Between append() and appendChild()

Both methods add content to the DOM.

```javascript
div.append("Hello");
```

```javascript
div.appendChild(paragraph);
```

| append()               | appendChild()      |
| ---------------------- | ------------------ |
| Adds text and elements | Adds only elements |
| Returns undefined      | Returns added node |

---

# 2. What Does concat() Do?

`concat()` combines arrays and returns a new array.

```javascript
const result = [1, 2].concat([3, 4]);
```

Output:

```text
[1, 2, 3, 4]
```

It is an immutable method.

---

# 3. Return Type of undefined

```javascript
console.log(typeof undefined);
```

Output:

```text
undefined
```

The type of `undefined` is `"undefined"`.

---

# 4. .then() and .catch() in Promises

`.then()` handles successful results.

`.catch()` handles errors.

```javascript
promise
  .then(data => console.log(data))
  .catch(error => console.log(error));
```

---

# 5. Common Promise Methods

```javascript
Promise.all()
Promise.race()
Promise.allSettled()
Promise.any()
```

These methods help manage multiple promises.

---

# 6. Higher Order Functions

A higher order function accepts another function as an argument or returns a function.

```javascript
numbers.map(num => num * 2);
```

Examples:

```javascript
map()
filter()
reduce()
forEach()
```

---

# 7. What is await?

`await` pauses an async function until a promise is resolved.

```javascript
const data = await fetchData();
```

It can only be used inside `async` functions.

---

# 8. querySelector vs querySelectorAll

```javascript
document.querySelector(".item");
```

Returns the first matching element.

```javascript
document.querySelectorAll(".item");
```

Returns all matching elements.

---

# 9. Return Type of null

```javascript
console.log(typeof null);
```

Output:

```text
object
```

This is a historical JavaScript behavior.

---

# 10. break vs continue

### break

Stops the loop completely.

```javascript
break;
```

### continue

Skips the current iteration.

```javascript
continue;
```

---

# 11. addEventListener vs onclick

```javascript
button.onclick = greet;
```

```javascript
button.addEventListener("click", greet);
```

| onclick        | addEventListener  |
| -------------- | ----------------- |
| One handler    | Multiple handlers |
| Older approach | Modern approach   |

---

# 12. Object.freeze()

Prevents modification of an object.

```javascript
Object.freeze(user);
```

Properties cannot be added, removed, or changed.

---

# 13. DOM vs CSSOM

### DOM

Represents HTML structure.

### CSSOM

Represents CSS styles.

Together they help browsers render web pages.

---

# 14. var vs let

| var               | let                  |
| ----------------- | -------------------- |
| Function scoped   | Block scoped         |
| Can be redeclared | Cannot be redeclared |
| Older syntax      | Modern syntax        |

Example:

```javascript
if (true) {
  let age = 25;
}

console.log(age);
```

Output:

```text
ReferenceError
```

---

