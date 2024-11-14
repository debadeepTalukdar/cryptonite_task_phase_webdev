# Introduction to CSS

CSS (Cascading Style Sheets) is a styling language used to define the visual appearance of HTML elements. It enables separation of content and presentation, which enhances maintainability and flexibility of web projects.

## Basic Example

HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>CSS Basics</title>
</head>
<body>
    <h1>Welcome to CSS</h1>
    <p>This is styled with CSS.</p>
</body>
</html>
```

```css
body {
    font-family: Arial, sans-serif;
    background-color: #e0f7fa;
}

h1 {
    color: #00796b;
}

p {
    color: #004d40;
}
```
### The Cascade Principle
The "cascade" defines how CSS rules are applied when multiple styles target the same element. The rules depend on importance, specificity, and source order.
```html
p {
    color: gray; /* Default style */
}

.important {
    color: red !important; /* Higher importance */
}

#special {
    color: blue; /* Higher specificity */
}
```
HTML
```html
<p class="important" id="special">This will be red due to !important.</p>
<p>Standard paragraph.</p>
```

#### Using Developer Tools
Most browsers offer Developer Tools for inspecting and modifying CSS live. Right-click an element, select "Inspect," and adjust styles directly in the browser to see real-time changes.

```html
<div class="container">
    <h2>Inspect Me</h2>
    <p>This section is styled with borders and spacing.</p>
</div>
```

```css
.container {
    border: 2px solid #00796b;
    padding: 15px;
    margin: 20px;
}
```

#### Understanding the Box Model
The CSS Box Model describes how elements are structured, consisting of content, padding, border, and margin.
```html
<div class="box-model-example">
    <h2>Box Model</h2>
</div>
```

```css
.box-model-example {
    width: 250px;
    padding: 10px; /* Space inside the border */
    border: 3px solid #004d40;
    margin: 20px; /* Space outside the element */
}
```

#### Block vs. Inline Elements
Block Elements
Block elements take up the full width available and start on a new line.
```html
<div class="block-example">
    <h3>Block Element</h3>
    <p>This is a block-level element.</p>
</div>
```

```css
.block-example {
    background-color: #b2dfdb;
    padding: 10px;
    margin-bottom: 10px;
}
```

#### Inline Elements
Inline elements take up only as much space as necessary and don't force line breaks.
```html
<span class="inline-example">Inline Element</span>
```
```css
.inline-example {
    color: #00796b;
    font-weight: bold;
}
```
#### Conclusion
CSS is essential for designing visually appealing web pages. Understanding the cascade, box model, and element display types helps in creating structured, maintainable layouts. Developer tools further enhance CSS workflows by providing a platform for quick experimentation and debugging



