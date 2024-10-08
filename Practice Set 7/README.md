# JavaScript Practice Set 7

## 1. Create a navbar and change the color of its first element to red.

### HTML Code:
```html
<nav>
    <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</nav>
```

### JavaScript Code:
```javascript
let navbar = document.querySelector("nav ul li");
navbar.style.color = "red"; // Change the color of the first element to red
```

### Explanation:
- This code selects the first `<li>` element inside the `<ul>` and changes its color to red.

---

## 2. Create a table without `<tbody>`. Use "View Page Source" to check if it has a `<tbody>` or not.

### HTML Code:
```html
<table>
    <tr>
        <td>Row 1, Cell 1</td>
        <td>Row 1, Cell 2</td>
    </tr>
    <tr>
        <td>Row 2, Cell 1</td>
        <td>Row 2, Cell 2</td>
    </tr>
</table>
```

### Task:
- After creating the table, right-click on the page and select "View Page Source" to check if the browser automatically adds the `<tbody>` tag. Most browsers will add `<tbody>` if it's missing.

---

## 3. Create an element with 3 children and change the color of the first and last elements to green.

### HTML Code:
```html
<div id="parent">
    <div>Child 1</div>
    <div>Child 2</div>
    <div>Child 3</div>
</div>
```

### JavaScript Code:
```javascript
let parent = document.getElementById("parent");
parent.firstElementChild.style.color = "green"; // First child to green
parent.lastElementChild.style.color = "green"; // Last child to green
```

### Explanation:
- The first and last child elements of the parent are selected using `firstElementChild` and `lastElementChild` and their colors are changed to green.

---

## 4. Write JavaScript code to change the background color of all `<li>` tags to cyan.

### HTML Code:
```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

### JavaScript Code:
```javascript
let listItems = document.querySelectorAll("li");

listItems.forEach((item) => {
    item.style.backgroundColor = "cyan"; // Change background to cyan
});
```

### Explanation:
- The code selects all `<li>` elements using `querySelectorAll` and iterates over them to change their background color to cyan.

---

## 5. Which of the following is used to look for a given CSS selector?

**(a) matches**
**(b) closest**
**(c) contains**
**(d) none of these**

### Answer:
**(d) none of these**

### Explanation:
- The `matches()` method checks whether an element itself matches a given CSS selector. It returns true if the element satisfies the selector, and false otherwise.
- The `closest()` method starts with the current element and traverses up through the DOM tree (its ancestors) to find the nearest ancestor that matches a given CSS selector. If no matching element is found, it returns null.
- The `contains()` method checks if one element contains another as a descendant. It returns true if the first element contains the second, otherwise false.