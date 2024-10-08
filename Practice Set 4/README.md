# JavaScript Practice Set 4

## 1. What will the following print in JavaScript?

### Code:
```javascript
console.log("har\"".length);
```

### Explanation:
- The string `"har\""` contains 5 characters: 
  - `h`, `a`, `r`, and an escaped double quote `\"`.
- The `.length` property returns the number of characters in the string.

### Output:
```
4
```

---

## 2. Explore the `includes()`, `startsWith()`, and `endsWith()` functions of a string.

### `includes()`
This method checks if a string contains a certain substring.

### Code:
```javascript
let str = "Hello World";
console.log(str.includes("World")); // Output: true
console.log(str.includes("world")); // Output: false (case-sensitive)
```

### `startsWith()`
This method checks if a string starts with a specific substring.

### Code:
```javascript
console.log(str.startsWith("Hello")); // Output: true
console.log(str.startsWith("World")); // Output: false
```

### `endsWith()`
This method checks if a string ends with a specific substring.

### Code:
```javascript
console.log(str.endsWith("World")); // Output: true
console.log(str.endsWith("Hello")); // Output: false
```

---

## 3. Write a program to convert a given string to lowercase.

### Code:
```javascript
let myString = "JavaScript is AWESOME!";
let lowerCaseString = myString.toLowerCase();

console.log(lowerCaseString); // Output: "javascript is awesome!"
```

---

## 4. Extract the amount out of this string: `"Please give Rs 1000"`.

### Code:
```javascript
let str = "Please give Rs 1000";
let amount = str.match(/\d+/); // This extracts the first set of digits

console.log(amount[0]); // Output: "1000"
```

Explanation: The `\d+` regex finds the first sequence of digits in the string.

---

## 5. Try to change the 4th character of a given string. Were you able to do it?

### Code:
```javascript
let myString = "JavaScript";
myString[3] = "X"; // Trying to change the 4th character

console.log(myString); // Output: "JavaScript"
```

### Explanation:
In JavaScript, strings are **immutable**, meaning you cannot directly change individual characters in a string. You would need to create a new string to achieve any changes.

---