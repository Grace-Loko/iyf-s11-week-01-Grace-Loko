# Semantic HTML and Accessibility: Building Better Websites

## Introduction
Semantic HTML is the practice of using HTML elements that clearly describe the purpose of the content on a webpage. Instead of using many `<div>` elements, semantic tags such as `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>` make the page easier to understand.
Semantic HTML is important because it improves accessibility, helps search engines understand web pages, and makes code easier to read and maintain.
---
## Before: Non-Semantic HTML
```html
<div class="header">
    <h1>My Portfolio</h1>
</div>
<div class="navigation">
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
</div>
<div class="content">
    <p>Welcome to my portfolio website.</p>
</div>
```
---
## After: Semantic HTML
```html
<header>
    <h1>My Portfolio</h1>
</header>
<nav>
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
</nav>
<main>
    <section>
        <p>Welcome to my portfolio website.</p>
    </section>
</main>
```
---
## Accessibility Issues I Found
### 1. Images Missing Alternative Text
Before:
```html
<img src="images/profile.jpg">
```
After:
```html
<img src="images/profile.jpg" alt="Profile picture of Grace Loko">
```
Adding alternative text allows screen readers to describe images to users with visual impairments.
---
### 2. Navigation Was Not Semantic
Before:
```html
<div>
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
</div>
```
After:
```html
<nav>
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
</nav>
```
Using the `<nav>` element helps assistive technologies identify the website navigation.
---
### 3. Form Inputs Had No Labels
Before:
```html
<input type="text" placeholder="Your Name">
```
After:
```html
<label for="name">Name</label>
<input type="text" id="name" name="name">
```
Labels improve accessibility by helping screen readers identify each form field.
---
## Conclusion
This accessibility audit helped me understand the importance of semantic HTML and accessible web design. By replacing non-semantic elements with semantic tags, adding image alt text, and using proper form labels, I made my portfolio more accessible and easier to use.
These improvements also make the website easier to maintain and improve the experience for all users.