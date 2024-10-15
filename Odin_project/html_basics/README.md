# HTML Learning Project

This project documents my knowledge in HTML. It covers the basics of HTML structure, text formatting, adding links and images, and following good commit practices.

## Table of Contents
- [1. Document Structure](#1-document-structure)
- [2. Editing and Formatting Text](#2-editing-and-formatting-text)
- [3. Adding Links and Images](#3-adding-links-and-images)
- [4. Commit Practices](#4-commit-practices)

---

## 1. Document Structure

### `<!DOCTYPE html>`
The `<!DOCTYPE html>` declaration tells the browser to interpret the document as an HTML5 document.

### `<html>`
The `<html>` element is the root of the document, which contains all other HTML elements.

### `<head>`
The `<head>` element contains metadata about the page, such as the title, character encoding, and links to stylesheets or scripts.

```html

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Project</title
</head>

```
## 2. Editing and Formatting Text

### Paragraphs (`<p>`)
The `<p>` element is used to define paragraphs of text.

### Headings (`<h1>` to `<h6>`)
Headings are used to structure the content, with `<h1>` being the most important (main heading) and `<h6>` being the least.

```html
<h1>Welcome to My Project</h1>
<p>This project explains various HTML concepts.</p>
<h2>Key Features</h2>
<p>Some features of this project include learning about headings, paragraphs, links, and images.</p>
```
### Text Formatting:
Bold: Use the <strong> or <b> tag to make text bold.
Italic: Use the <em> or <i> tag to italicize text
```html
<p>This is <strong>bold</strong> and this is <em>italic</em>.</p>
```

### 3. Adding Links and Images
### Links
To create links to other websites or pages, use the <a> element.
```html
<h1>Welcome to My Project</h1>
<p>This project explains various HTML concepts.</p>
<h2>Key Features</h2>
<p>Some features of this project include learning about headings, paragraphs, links, and images.</p>
```
we can also use target attribute to open this to new a page 
we can use absolute links for linking to external websites.
we can use relative links for linking to internal pages on the same website.
### Images
To display an image, use the <img> element with the src attribute.

```html

<img src="https://example.com/image.jpg" alt="Example Image">

```


### 4. Commit Practices
Good Commit Practices
Write clear, concise commit messages that accurately describe changes.
Focus each commit on a single feature or task.
Example of a good commit message:

arduino
Copy code
Added text formatting and image display functionality.
Bad Commit Practices
Avoid vague messages like "Fixed stuff" or "Updated".
Don’t combine unrelated changes in a single commit.
Example of a bad commit message:

Copy code
Updated things
