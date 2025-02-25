# CSS Notes

## Introduction to CSS
CSS (Cascading Style Sheets) is used to style HTML elements and control the layout of web pages.

## Selectors
- **Element Selector**: Targets all elements of a specific type.  
  ```css
  p {
    color: blue;
  }
  ```
- **Class Selector**: Targets elements with a specific class.  
  ```css
  .my-class {
    font-size: 16px;
  }
  ```
- **ID Selector**: Targets a single element with a specific ID.  
  ```css
  #my-id {
    background-color: yellow;
  }
  ```
- **Universal Selector**: Targets all elements.  
  ```css
  * {
    margin: 0;
    padding: 0;
  }
  ```
- **Attribute Selector**: Targets elements with a specific attribute.  
  ```css
  input[type="text"] {
    border: 1px solid black;
  }
  ```

## Pseudo-Classes
Pseudo-classes define a special state of an element.
```css
button:hover {
  background-color: lightblue;
}
```
Common pseudo-classes:
- `:hover` - When a user hovers over an element.
- `:focus` - When an element is focused.
- `:nth-child(n)` - Targets the nth child of a parent element.
- `:first-child` / `:last-child` - Targets the first or last child of a parent.

## Pseudo-Elements
Pseudo-elements style specific parts of an element.
```css
p::first-letter {
  font-size: 2em;
  color: red;
}
```
Common pseudo-elements:
- `::before` - Inserts content before an element.
- `::after` - Inserts content after an element.
- `::first-letter` - Styles the first letter of an element.
- `::first-line` - Styles the first line of an element.

## Box Model
Each element in CSS has a box model consisting of:
1. **Content**: The actual content (text, images, etc.).
2. **Padding**: Space between content and border.
3. **Border**: Surrounds padding and content.
4. **Margin**: Space outside the border.

```css
.box {
  width: 200px;
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
}
```

## CSS Units and Sizes
CSS provides different units for defining sizes:
- **Absolute Units** (Fixed sizes)
  - `px` (Pixels): Fixed unit, does not scale with user settings.
  - `pt` (Points): Typically used for print styles.
  - `cm`, `mm`, `in` (Centimeters, Millimeters, Inches): Rarely used in web design.

- **Relative Units** (Scalable sizes)
  - `em`: Relative to the font-size of the parent element.
  - `rem`: Relative to the font-size of the root element (`html`).
  - `%`: Relative to the parent element's size.
  - `vh` / `vw`: Viewport height and width, relative to the screen size.
  - `vmin` / `vmax`: Relative to the smaller or larger viewport dimension.

Example usage:
```css
body {
  font-size: 16px;
}
p {
  font-size: 1.5em; /* 1.5 times the parent's font size */
}
h1 {
  font-size: 2rem; /* 2 times the root font size */
}
.container {
  width: 80vw; /* 80% of the viewport width */
}
```

## Flexbox
Used to create responsive layouts efficiently.
```css
.container {
  display: flex;
  justify-content: center; /* Aligns items horizontally */
  align-items: center; /* Aligns items vertically */
}
```

## Grid
CSS Grid is another layout system for creating complex designs.
```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}
```

## Responsive Design
- **Media Queries**: Apply styles based on screen size.
```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

## Animations
- **Transitions**: Smoothly changes a property over time.
```css
.button {
  transition: background-color 0.3s ease;
}
```
- **Keyframes**: Create complex animations.
```css
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
```

## Learn More
For more details, visit the [MDN Web Docs on CSS](https://developer.mozilla.org/en-US/docs/Web/CSS).

---
