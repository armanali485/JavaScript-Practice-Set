# JavaScript Practice Set 3

## 1. Write an object using:
Create an object with key-value pairs where the keys are names and the values are their respective scores.

### Code:
```javascript
let marks = {
    harry: 98,
    rohan: 70,
    aakash: 7
};

console.log(marks); // Output: { harry: 98, rohan: 70, aakash: 7 }
```

This object stores the scores of `harry`, `rohan`, and `aakash`.

---

## 2. Write the program in 1 using a `for-in` loop.
The `for-in` loop allows you to iterate over the keys in an object.

### Code:
```javascript
let marks = {
    harry: 98,
    rohan: 70,
    aakash: 7
};

for (let student in marks) {
    console.log(`${student}: ${marks[student]}`);
}
```

This program will print each student’s name along with their marks:
```
harry: 98
rohan: 70
aakash: 7
```

---

## 3. Write a program to print "try again" until the user enters the correct number.

You can create a loop to repeatedly ask the user to enter a number until the correct number is entered.

### Code:
```javascript
let correctNumber = 42;
let userGuess;

while (userGuess != correctNumber) {
    userGuess = prompt("Enter a number: ");
    if (userGuess != correctNumber) {
        console.log("Try again!");
    }
}

console.log("Congratulations! You've guessed the correct number.");
```

In this program, the user is prompted to enter a number until they guess the correct number (`42`).

---

## 4. Write a function to find the mean of 5 numbers.

Create a function that accepts 5 numbers as arguments and returns their mean (average).

### Code:
```javascript
function findMean(a, b, c, d, e) {
    return (a + b + c + d + e) / 5;
}

console.log(findMean(5, 10, 15, 20, 25)); // Output: 15
```

This function calculates the mean of the 5 numbers passed as arguments.

---