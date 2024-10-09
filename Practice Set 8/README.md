# JavaScript Practice Set 8

## 1. Write a program to show different buttons that trigger different alerts.
This task isn't directly shown in the provided files, but you can modify the code below to display different alert messages when buttons are clicked.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Button Alerts</title>
</head>
<body>
    <button id="btn1">Button 1</button>
    <button id="btn2">Button 2</button>
    <button id="btn3">Button 3</button>

    <script>
        document.getElementById("btn1").addEventListener("click", function() {
            alert("Button 1 Clicked!");
        });
        document.getElementById("btn2").addEventListener("click", function() {
            alert("Button 2 Clicked!");
        });
        document.getElementById("btn3").addEventListener("click", function() {
            alert("Button 3 Clicked!");
        });
    </script>
</body>
</html>
```

---

## 2. Create a bookmarks website capable of storing your favorite websites using `href`.

The `2.html` and `3.html` files you provided have JavaScript that sets button links dynamically. Here’s the extracted version from **[41†source]**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bookmarks</title>
</head>
<body>
    <button>Google</button>
    <button>YouTube</button>
    <button>Telegram</button>
    <button>Instagram</button>

    <script>
        let a = document.getElementsByTagName("button");
        let buttonArray = Array.from(a);
        let links = [
            "https://www.google.com/",
            "https://www.youtube.com/",
            "https://web.telegram.org/",
            "https://www.instagram.com/"
        ];
        let setButtonLinks = (element, index) => {
            element.addEventListener("click", () => {
                location.href = links[index];
            });
        };
        buttonArray.forEach(setButtonLinks);
    </script>
</body>
</html>
```

---

## 3. Repeat task 2 using event listeners.

This task is already handled in **[42†source]**, where the JavaScript dynamically assigns event listeners to buttons that redirect users to favorite websites.

---

## 4. Write a JavaScript program to keep fetching the contents of a website every 5 seconds.

You can simulate fetching website content by updating the DOM every 5 seconds using `setInterval`. Here's a basic example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Content Fetcher</title>
</head>
<body>
    <div id="content">Fetching content...</div>

    <script>
        setInterval(() => {
            document.getElementById("content").innerHTML = "Updated content at " + new Date().toLocaleTimeString();
        }, 5000); // Fetch content every 5 seconds
    </script>
</body>
</html>
```

---

## 5. Create a glowing bulb effect using the `classList.toggle()` method in JavaScript.

The glowing bulb effect is provided in **[43†source]**. Here’s the code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Glowing Bulb</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        body {
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        #bulb {
            border-radius: 50%;
            height: 300px;
            width: 300px;
            border: 2px solid black;
            background-color: yellow;
        }
        .bulbOn {
            box-shadow: 0 0 90px 50px yellow;
        }
    </style>
</head>
<body>
    <div id="bulb"></div>

    <script>
        setInterval(() => {
            document.getElementById("bulb").classList.toggle("bulbOn");
        }, 300); // Toggle the glowing effect every 300ms
    </script>
</body>
</html>
```