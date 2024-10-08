# JavaScript Practice Set 6

## 1. Write a program to take user input of age using the `prompt` function and alert the user to tell him if he can drive.

### Code:
```javascript
let age = prompt("Please enter your age:");

if (age >= 18) {
    alert("You can drive!");
} else {
    alert("You cannot drive!");
}
```

### Explanation:
- The program prompts the user to enter their age and then checks if the age is 18 or above. An alert displays whether the user can drive.

---

## 2. In Q1, use `confirm` to ask the user if they want to see the prompt again.

### Code:
```javascript
let canSeePrompt = true;

while (canSeePrompt) {
    let age = prompt("Please enter your age:");

    if (age >= 18) {
        alert("You can drive!");
    } else {
        alert("You cannot drive!");
    }

    canSeePrompt = confirm("Do you want to see the prompt again?");
}
```

### Explanation:
- This version uses a `while` loop to continuously prompt the user for their age until they choose not to see the prompt again using the `confirm` dialog.

---

## 3. In the previous question, use `console.error` to log an error if the age entered is negative.

### Code:
```javascript
let canSeePrompt = true;

while (canSeePrompt) {
    let age = prompt("Please enter your age:");

    if (age < 0) {
        console.error("Age cannot be negative.");
        alert("Please enter a valid age.");
        continue; // Skip to the next iteration if age is negative
    }

    if (age >= 18) {
        alert("You can drive!");
    } else {
        alert("You cannot drive!");
    }

    canSeePrompt = confirm("Do you want to see the prompt again?");
}
```

### Explanation:
- The program checks if the entered age is negative. If so, it logs an error message to the console using `console.error()` and prompts the user to enter a valid age.

---

## 4. Write a program to change the URL to `google.com` if the user enters a number greater than 4.

### Code:
```javascript
let number = prompt("Enter a number:");

if (number > 4) {
    window.location.href = "https://www.google.com"; // Redirect to Google
}
```

### Explanation:
- If the user enters a number greater than 4, the program redirects them to Google by changing the `window.location.href`.

---

## 5. Change the background color of the page based on user input through a prompt.

### Code:
```javascript
let color = prompt("Enter a color for the background:");

document.body.style.backgroundColor = color; // Change the background color
```

### Explanation:
- The user is prompted to enter a color, and the program sets the background color of the document to that color.

---