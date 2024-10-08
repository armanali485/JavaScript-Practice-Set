# JavaScript Practice Set 5

## 1. Create an array of numbers and take input from the user to add numbers to this array.

In JavaScript, you can prompt the user for input and push the numbers into an array.

### Code:
```javascript 
let numbersArray = [];
let userInput = prompt("Enter a number to add to the array (enter 0 to stop):");

while (parseInt(userInput) !== 0) {
    numbersArray.push(parseInt(userInput));
    userInput = prompt("Enter a number to add to the array (enter 0 to stop):");
}

console.log(numbersArray); // Output: The array with user inputs
```

Explanation: This program will keep asking the user to enter numbers and add them to `numbersArray` until the user inputs `0`.

---

## 2. Keep adding numbers to the array in Task 1 until the array contains 0.

This is already demonstrated in Task 1 above, where we keep adding numbers until `0` is input by the user.

---

## 3. Filter numbers divisible by 10 from the array.

Using the `filter()` method, we can extract numbers divisible by 10.

### Code:
```javascript
let divisibleBy10 = numbersArray.filter((num) => num % 10 === 0);
console.log(divisibleBy10); // Output: An array of numbers divisible by 10
```

Explanation: The `filter()` function checks each number in the array and returns only those divisible by 10.

---

## 4. Create an array of squares of the given numbers.

Using the `map()` method, we can create an array of the squares of the numbers from `numbersArray`.

### Code:
```javascript
let squaresArray = numbersArray.map((num) => num * num);
console.log(squaresArray); // Output: An array of squares of the original numbers
```

Explanation: The `map()` function applies the square operation to each element of the array.

---

## 5. Use `reduce()` to calculate the factorial of a given number from an array of the first n natural numbers.

To calculate the factorial of a number, you can use the `reduce()` method on an array of the first n natural numbers.

### Code:
```javascript
let n = 5; // For example, calculating factorial of 5
let naturalNumbers = Array.from({ length: n }, (_, i) => i + 1);

let factorial = naturalNumbers.reduce((acc, num) => acc * num, 1);
console.log(`Factorial of ${n}:`, factorial); // Output: 120 for n = 5
```

Explanation: 
- `Array.from()` creates an array of the first `n` natural numbers.
- `reduce()` multiplies all the numbers in the array to compute the factorial.

---