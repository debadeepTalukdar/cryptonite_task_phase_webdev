##### CSS Flexbox Module

Flexbox, or the **Flexible Box Layout**, is a layout model in CSS that allows you to design complex layouts with simple and clean code. It enables easy alignment and distribution of space among items in a container, even when the size of items is unknown or dynamic.


#### flex-direction
Sets the direction of the flex items (row or column).

row (default): Items are laid out in a horizontal row.
column: Items are laid out in a vertical column.
row-reverse: Items are laid out in reverse order in a horizontal row.
column-reverse: Items are laid out in reverse order in a vertical column

```css
.container {
  flex-direction: row;
}
flex-wrap
Controls whether flex items are forced into a single line or can wrap into multiple lines.
```
```css
Copy code
.container {
  flex-wrap: wrap;
}
```

#### Aligns flex items along the main axis (horizontal or vertical depending on flex-direction).

flex-start: Items align at the start.
flex-end: Items align at the end.
center: Items align at the center.
space-between: Items are spaced evenly with the first item at the start and the last at the end.
space-around: Items are spaced evenly with equal space around them.
```css

.container {
  justify-content: center;
}
```
align-items
Aligns flex items along the cross axis (perpendicular to the main axis).

#### stretch: Items stretch to fill the container (default).
flex-start: Items align at the start of the cross axis.
flex-end: Items align at the end of the cross axis.
center: Items align in the center of the cross axis.
baseline: Items align based on their text baseline.
```css

.container {
  align-items: center;
}
```
#### align-content
Aligns rows of items when there is extra space in the container.

flex-start: Align rows to the start.
flex-end: Align rows to the end.
center: Align rows in the center.
space-between: Evenly distribute rows with the first at the start and the last at the end.
space-around: Evenly distribute rows with equal space around them.
```css
.container {
  align-content: space-between;
}
```
#### Flexbox Item Properties
flex-grow
Defines the ability for a flex item to grow if necessary. The default value is 0, meaning it will not grow.

```css

.item {
  flex-grow: 1;
}
```
#### flex-shrink
Defines the ability for a flex item to shrink if necessary. The default value is 1, meaning it will shrink if needed.

```css
.item {
  flex-shrink: 1;
}
```
#### flex-basis
Defines the initial size of a flex item before any growing or shrinking occurs.

```css

.item {
  flex-basis: 100px;
}
```
### flex
A shorthand for flex-grow, flex-shrink, and flex-basis.

```css
.item {
  flex: 1 1 100px; /* grow, shrink, basis */
}
```
#### align-self
Allows a flex item to override the align-items value for its own alignment along the cross axis.

```css
.item {
  align-self: center;
}
```
#### Practical Examples
Centering Items
To center items both horizontally and vertically within a container:

```css

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* Full viewport height */
}
```
#### Equal Width Columns
To create a layout with equal-width columns:

```css
.container {
  display: flex;
}

.item {
  flex: 1;
  padding: 10px;
}
```
#### Browser Support
Flexbox is supported in all modern browsers. Ensure to check compatibility for older browsers like Internet Explorer if needed.

Browser	Version
Chrome	29+
Firefox	28+
Safari	9+
Edge	12+
Internet Explorer	10 (partial support)
This guide covers the essentials of the CSS Flexbox module. Flexbox is a powerful tool for responsive design and layout management. Experiment with the properties to create flexible, dynamic layouts.
