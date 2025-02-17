# HTML Notes

## 1. Document Structure

### Basic HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My HTML Notes</title>
</head>
<body>
    <h1>Welcome to My HTML Notes</h1>
</body>
</html>
```

## 2. Headings and Paragraphs

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Heading</h3>
<p>This is a paragraph with <strong>bold</strong> and <i>italic</i> text.</p>
```

## 3. Lists

### Ordered List
```html
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

### Unordered List
```html
<ul>
    <li>Item One</li>
    <li>Item Two</li>
    <li>Item Three</li>
</ul>
```

## 4. Links and Anchors
```html
<a href="https://www.example.com">Visit Example</a>
<a href="#section2">Jump to Section 2</a>
```

## 5. Media Elements

### Images
```html
<img src="image.jpg" alt="A descriptive text about the image">
```

### Audio
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>
```

### Video
```html
<video controls width="600">
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

### Picture (Responsive Images)
```html
<picture>
    <source srcset="small.jpg" media="(max-width: 600px)">
    <source srcset="large.jpg" media="(min-width: 601px)">
    <img src="fallback.jpg" alt="A responsive image">
</picture>
```

### Figure and Figcaption
```html
<figure>
    <img src="image.jpg" alt="An image description">
    <figcaption>This is a caption for the image.</figcaption>
</figure>
```

## 6. Forms and Inputs
```html
<form action="submit.php" method="POST">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    
    <label for="message">Message:</label>
    <textarea id="message" name="message"></textarea>
    
    <button type="submit">Submit</button>
</form>
```

## 7. Tables
```html
<table border="1">
    <thead>
        <tr>
            <th>Name</th>
            <th>Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>John</td>
            <td>25</td>
        </tr>
        <tr>
            <td>Jane</td>
            <td>30</td>
        </tr>
    </tbody>
</table>
```

## 8. Semantic and Structural Elements

### When to Use Different Structural Elements

#### `<div>`
- Used as a generic container for grouping elements.
- Commonly used for styling purposes.

```html
<div class="container">
    <h2>Section Title</h2>
    <p>This is some content inside a div.</p>
</div>
```

#### `<section>`
- Used to group related content together.
- Ideal for dividing different sections of a webpage.

```html
<section>
    <h2>About Us</h2>
    <p>Information about the company.</p>
</section>
```

#### `<article>`
- Represents a self-contained piece of content.
- Useful for blog posts, news articles, or standalone content.

```html
<article>
    <h2>Blog Post Title</h2>
    <p>This is a standalone blog post.</p>
</article>
```

#### `<aside>`
- Used for content related to the main content but not part of it.
- Commonly used for sidebars, advertisements, or related links.

```html
<aside>
    <h3>Related Articles</h3>
    <ul>
        <li><a href="#">Article 1</a></li>
        <li><a href="#">Article 2</a></li>
    </ul>
</aside>
```

#### `<header>`
- Used to define introductory content or navigation links.
- Can be used inside `<article>` and `<section>` as well.

```html
<header>
    <h1>Website Header</h1>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
        </ul>
    </nav>
</header>
```

#### `<footer>`
- Defines footer content, such as copyright information or additional links.

```html
<footer>
    <p>&copy; 2025 My Website</p>
</footer>
```

## 9. Buttons
```html
<button>Click Me</button>
<input type="button" value="Click Me">
```

## 10. Iframes
```html
<iframe src="https://www.example.com" width="600" height="400"></iframe>
```

This markdown file can be used as a reference while working with HTML.
