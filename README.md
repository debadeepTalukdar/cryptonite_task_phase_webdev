#### ASSIGNMENT
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flexbox Examples</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <h1>Flexbox Examples</h1>

  <!-- Centering Items Example -->
  <section class="container-center">
    <div class="item">Centered Item</div>
  </section>

  <!-- Equal Width Columns Example -->
  <section class="container-columns">
    <div class="item">Column 1</div>
    <div class="item">Column 2</div>
    <div class="item">Column 3</div>
  </section>

  <!-- Flex Direction and Wrapping Example -->
  <section class="container-wrap">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
    <div class="item">Item 4</div>
    <div class="item">Item 5</div>
  </section>

</body>
</html>
```

```css
/* General styles for items */
.item {
  background-color: #4CAF50;
  color: white;
  padding: 20px;
  margin: 10px;
  text-align: center;
  border-radius: 5px;
}

/* Centering Items Example */
.container-center {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  background-color: #f2f2f2;
  margin-bottom: 20px;
}

/* Equal Width Columns Example */
.container-columns {
  display: flex;
  justify-content: space-around;
  background-color: #f2f2f2;
  padding: 20px;
}

.container-columns .item {
  flex: 1;
  padding: 20px;
}

/* Flex Direction and Wrapping Example */
.container-wrap {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  background-color: #f2f2f2;
  padding: 20px;
  gap: 10px;
}

/* Additional Examples of Flexbox Properties */

/* Justify content example */
.container-wrap {
  justify-content: space-between;
}

/* Align items example */
.container-wrap {
  align-items: center;
}

/* Individual item grow, shrink, and basis */
.item:nth-child(1) {
  flex: 1 1 100px; /* Grow, shrink, and basis */
}
```
#### Explanation of Key Properties
Centering Items: .container-center centers its item both horizontally and vertically.
Equal Width Columns: .container-columns has flex: 1 on each item to distribute them evenly in columns.
Flex Direction and Wrapping: .container-wrap demonstrates wrapping and alignment with flex-direction: row, flex-wrap: wrap, and justify-content
