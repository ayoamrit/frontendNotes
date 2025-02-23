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

## Advanced Concepts
### CSS Variables
Define reusable values.
```css
:root {
  --primary-color: blue;
}
.button {
  background-color: var(--primary-color);
}
```

### CSS Grid Advanced
Using named grid areas.
```css
.grid {
  display: grid;
  grid-template-areas: "header header"
                       "sidebar content";
}
.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.content { grid-area: content; }
```

### Clipping and Masking
Control visibility of elements.
```css
.clip {
  clip-path: circle(50% at center);
}
```

### CSS Transforms
Apply transformations to elements.
```css
.box {
  transform: rotate(45deg);
}
```

## Learn More
For more details, visit the [MDN Web Docs on CSS](https://developer.mozilla.org/en-US/docs/Web/CSS).

