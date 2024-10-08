# JavaScript Practice Set 2

## 1. Use logical operators to find whether the age of a person lies between 10 and 20.

In JavaScript, we can use logical operators (`&&`) to check if a person's age lies between 10 and 20.

### Code:
```javascript
let age = 15;
if (age >= 10 && age <= 20) {
    console.log("The age lies between 10 and 20.");
} else {
    console.log("The age does not lie between 10 and 20.");
}
```

This checks whether the variable `age` is greater than or equal to 10 and less than or equal to 20.

---

## 2. Demonstrate the use of switch case statements in JavaScript.

The `switch` statement evaluates an expression and executes code depending on the result.

### Code:
```javascript
let day = 3;
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    default:
        console.log("Invalid day");
}
```

This program checks the value of `day` and prints the corresponding day of the week.

---

## 3. Write a JavaScript program to find whether a number is divisible by 2 and 3.

Using the modulus operator `%`, we can check if a number is divisible by both 2 and 3.

### Code:
```javascript
let number = 12;
if (number % 2 === 0 && number % 3 === 0) {
    console.log(`${number} is divisible by both 2 and 3.`);
} else {
    console.log(`${number} is not divisible by both 2 and 3.`);
}
```

---

## 4. Write a JavaScript program to find whether a number is divisible by 2 or 3.

Here, we use the logical `OR` operator (`||`) to check divisibility by either 2 or 3.

### Code:
```javascript
let number = 9;
if (number % 2 === 0 || number % 3 === 0) {
    console.log(`${number} is divisible by 2 or 3.`);
} else {
    console.log(`${number} is not divisible by 2 or 3.`);
}
```

---

## 5. Print whether "You Can Drive" or "You Cannot Drive" based on age being greater than 18 using a ternary operator.

A ternary operator provides a concise way to check conditions and return values.

### Code:
```javascript
let age = 19;
let canDrive = (age >= 18) ? "You Can Drive" : "You Cannot Drive";
console.log(canDrive); // Output: "You Can Drive"
```

In this example, the program checks if the age is 18 or greater and prints the appropriate message.

---