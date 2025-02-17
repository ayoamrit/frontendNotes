# HTML Notes
<p>HTML is an incredibly important part of the web. If you use the right HTML element for the right job, you start from a place of great strength. Making your project understandable to voice interfaces, search engines, social media. Using the power that's built right into the browser for a variety of devices and users. <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" alt="Link to the MDN Website" target="_blank">MDN</a></p>

## 1. Document Structure

### Basic HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="location" rel="relation">
    <title>My HTML Notes</title>
</head>
<body>
    <h1>Welcome to My HTML Notes</h1>
</body>
</html>
```

## 2. Headings, Paragraphs & Text

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Heading</h3>
<p>This is a paragraph with <strong>bold</strong> and <i>italic</i> text.</p>
<u>Underlined Text</u>
<small>Small text</small>
<sup>Superscript</sup>
<sub>Subscript</sub>
<pre>Display text as-is, preserving spaces and line breaks</pre>
<code>Represents inline code snippets</code>
<blockquote>For long quotations </blockquote>
<q>Inline short quotes</q>
<cite>Citation for a source</cite>
<abbr>Abbreviations (show full form on hover)</abbr>
<dfn>Definition term</dfn>
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
<a href="https://www.example.com" alt="Example" target="_blank">Visit Example</a>
<a href="#section2" rel="relationship between pages">Jump to Section 2</a>
```

## 5. Media Elements

### Images
```html
<img src="image.jpg" alt="A descriptive text about the image" width="100" height="100">
```

### Audio
```html
<audio controls autoplay loop muted>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>
```

### Video
```html
<video controls width="600" autoplay loop muted>
    <source src="video.mp4" type="video/mp4">
    <track src="caption.vtt" kind="captions" label="english" srclang="en" default>
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
    <input type="text" id="name" name="name" placeholder="hint inside input" disabled readonly maxlength="10" required>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" minlength="6" required>
    
    <label for="phone">Phone:</label>
    <input type="tel" id="phone" name="phone" pattern="[0-9]{10}" required>
    
    <label for="url">Website:</label>
    <input type="url" id="url" name="url">
    
    <label for="number">Number:</label>
    <input type="number" id="number" name="number" min="1" max="100">
    
    <label for="date">Date:</label>
    <input type="date" id="date" name="date">
    
    <label for="time">Time:</label>
    <input type="time" id="time" name="time">
    
    <label for="datetime">Datetime:</label>
    <input type="datetime-local" id="datetime" name="datetime">
    
    <label for="color">Color:</label>
    <input type="color" id="color" name="color">
    
    <label for="range">Range:</label>
    <input type="range" id="range" name="range" min="0" max="100">
    
    <label for="file">Upload File:</label>
    <input type="file" id="file" name="file">
    
    <label for="message">Message:</label>
    <textarea id="message" name="message"></textarea>
    
    <fieldset>
        <legend>Gender:</legend>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
        <input type="radio" id="other" name="gender" value="other">
        <label for="other">Other</label>
    </fieldset>
    
    <fieldset>
        <legend>Hobbies:</legend>
        <input type="checkbox" id="reading" name="hobby" value="reading">
        <label for="reading">Reading</label>
        <input type="checkbox" id="sports" name="hobby" value="sports">
        <label for="sports">Sports</label>
        <input type="checkbox" id="music" name="hobby" value="music">
        <label for="music">Music</label>
    </fieldset>
    
    <label for="cars">Choose a car:</label>
    <select id="cars" name="cars">
        <option value="volvo">Volvo</option>
        <option value="bmw">BMW</option>
        <option value="audi">Audi</option>
    </select>
    
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
