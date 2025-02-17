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
<p>This is a paragraph with <strong>bold</strong> and <em>italic</em> text.</p>
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

## 8. Semantic Elements
```html
<header>
    <h1>Website Header</h1>
</header>
<nav>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
    </ul>
</nav>
<main>
    <article>
        <h2>Article Title</h2>
        <p>This is a sample article.</p>
    </article>
</main>
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

This markdown file can be used as a reference while working with HTML. Let me know if you want any modifications or additional sections!
