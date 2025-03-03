# jQuery Introduction & Setup

## 📌 What is jQuery?

jQuery is a fast, small, and feature-rich JavaScript library that simplifies HTML document traversal, event handling, animation, and AJAX interactions. It provides an easy-to-use API that works across multiple browsers.

### 🚀 Key Features of jQuery:
- **DOM Manipulation** – Easily select and modify elements in the DOM.
- **Event Handling** – Handle events like clicks, form submissions, and keypresses with minimal code.
- **AJAX Support** – Make asynchronous requests without reloading the page.
- **Animations & Effects** – Create smooth animations with built-in methods.
- **Cross-Browser Compatibility** – Works seamlessly across different browsers.

---

## 📌 How to Include jQuery in Your Project

### 🔹 Method 1: Using a CDN (Content Delivery Network)
This is the easiest way to include jQuery without downloading anything.

Add the following script tag inside your HTML file:

```html
<!-- Include jQuery from a CDN -->
<script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
```

### 🔹 Method 2: Download & Use Locally
1. Go to [jQuery's official website](https://jquery.com/).
2. Download the latest version.
3. Place the `jquery.min.js` file in your project folder.
4. Include it in your HTML file:

```html
<script src="path/to/jquery.min.js"></script>
```

---

## 📌 Installing jQuery via NPM & Yarn

For projects using Node.js, you can install jQuery via package managers.

### 🔹 Using NPM:
```sh
npm install jquery
```

### 🔹 Using Yarn:
```sh
yarn add jquery
```

To use jQuery in your JavaScript file after installing it via NPM or Yarn:
```js
import $ from 'jquery';
$(document).ready(function() {
    console.log("jQuery is ready to use!");
});
```

---

## 📌 Basic Example of jQuery Usage

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>jQuery Example</title>
    <script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
</head>
<body>
    <button id="btn">Click Me</button>
    <p id="text">Hello, jQuery!</p>

    <script>
        $(document).ready(function() {
            $("#btn").click(function() {
                $("#text").toggle();
            });
        });
    </script>
</body>
</html>
```

### Explanation:
- The `$` symbol represents jQuery.
- `$(document).ready(function() {...})` ensures the script runs only after the document is fully loaded.
- `$("#btn").click(function() {...})` binds a click event to the button.
- `$("#text").toggle();` hides/shows the paragraph on each click.

---

This README provides an introduction and setup guide for jQuery. Stay tuned for more advanced topics like event handling, AJAX, and animations! 🚀

