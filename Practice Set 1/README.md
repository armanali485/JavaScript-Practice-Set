# JavaScript Practice Set 1

## 1. Create a variable of type string and try to add a number to it.
When a number is added to a string in JavaScript, the number is implicitly converted to a string, and the result is a concatenation.

### Code:
```javascript
let myString = "Hello";
let myNumber = 5;
let result = myString + myNumber;
console.log(result); // Output: "Hello5"
```

In this case, the number `5` is converted to the string `"5"`, and the result becomes `"Hello5"`.

## 2. Use the `typeof` operator twice to find the data type of the string from the last question.
The `typeof` operator is used to determine the type of a variable or expression.

### Code:
```javascript
console.log(typeof result);   // Output: "string"
console.log(typeof myString); // Output: "string"
```

Both `result` and `myString` are strings, so the `typeof` operator will return `"string"`.

## 3. Create a `const` object in JavaScript. Can you change a `const` to a number later?
A `const` object cannot be reassigned, but its properties can be modified. Reassigning a `const` to a number will result in an error.

### Code:
```javascript
const myObject = { key: "value" };
// Trying to reassign will throw an error:
// myObject = 42; // This will cause an error
```

## 4. Try to add a new key to the `const` object in Problem 3. Were you able to do it?
Yes, you can add new properties to a `const` object, but you cannot reassign the object itself.

### Code:
```javascript
myObject.newKey = "newValue";
console.log(myObject); // Output: { key: "value", newKey: "newValue" }
```

In this case, we successfully added a new key `newKey` to the `const` object.

## 5. Write a dictionary of programs to create a word-meaning dictionary.
You can create a simple JavaScript object to store words and their meanings, essentially functioning as a dictionary.

### Code:
```javascript
const dictionary = {
  "JavaScript": "A programming language used for web development.",
  "Node.js": "A JavaScript runtime built on Chrome's V8 engine.",
  "MERN": "A stack that includes MongoDB, Express, React, and Node.js."
};

console.log(dictionary["JavaScript"]); // Output: A programming language used for web development.
console.log(dictionary["Node.js"]);    // Output: A JavaScript runtime built on Chrome's V8 engine.
```

This object allows you to look up words and their meanings using the key-value pair structure.

---
