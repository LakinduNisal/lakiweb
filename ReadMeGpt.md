This HTML code is structured to create a modern, visually appealing personal website. Let's go through each section step by step to understand what each part does.

### 1. `<!DOCTYPE html>`
Defines the document type, which helps browsers to interpret it as HTML5.

### 2. `<html lang="en">`
The root element of the document, where `lang="en"` specifies the language (English).

### 3. `<head>`
The `<head>` section contains metadata about the document, including styles, scripts, and the document title.

- `<meta charset="UTF-8">`: Sets the character encoding to UTF-8, supporting most characters and symbols.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Ensures responsive design, adjusting the layout on mobile devices.
- `<title>Lakindu Nisal</title>`: Specifies the webpage title, appearing in the browser tab.
- `<script src="https://cdn.tailwindcss.com"></script>`: Loads Tailwind CSS, a utility-first CSS framework.
- `<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>`: Loads GSAP (GreenSock Animation Platform) for animations.

### 4. `<style>`
Contains custom CSS styles:
- `.gradient-text`: Creates a gradient text effect.
- `.card`: Sets a default transform style for cards, with a hover effect to slightly lift them.
- `.animate-float`: Applies a floating animation using `@keyframes float`.
- `.welcome-overlay` and `.welcome-text`: Adds a welcome overlay that fades out with animation after the page loads.

### 5. `<body class="bg-[#0a0a0a] text-white">`
The `<body>` tag contains all visible content on the webpage. Here, a dark background (`bg-[#0a0a0a]`) and white text (`text-white`) are applied using Tailwind CSS classes.

### 6. Welcome Overlay
```html
<div class="welcome-overlay">
    <h1 class="welcome-text gradient-text font-bold">Welcome to My World</h1>
</div>
```
This section displays an overlay with a "Welcome to My World" message that fades out after two seconds.

### 7. Navigation Bar
```html
<nav class="fixed w-full bg-[#0a0a0a] bg-opacity-90 backdrop-filter backdrop-blur-lg z-50">
```
- The navbar is fixed at the top (`fixed`), with a semi-transparent background and blur effect.
- Links (`About`, `Passions`, etc.) lead to sections on the same page.

### 8. Mobile Menu
```html
<div id="mobileMenu" class="fixed inset-0 bg-[#0a0a0a] bg-opacity-95 z-40 hidden">
```
- The `mobileMenu` is a full-screen overlay for navigation links on smaller screens.
- Initially hidden, it displays on button click with `toggleMenu()`.

### 9. Hero Section
```html
<section class="min-h-screen flex items-center justify-center pt-20">
```
This section introduces "Lakindu Nisal" with a title, description, and floating profile image. Highlights include:
- `Hi, I'm Lakindu Nisal` with a gradient effect.
- A button to "Get in Touch," linking to the `connect` section.
- The profile image, animated with a floating effect (`animate-float`).

### 10. About Section
```html
<section id="about" class="py-20">
```
Provides information on Lakindu’s background, current academic focus, and career aspirations. The section is divided into:
- Descriptive paragraphs.
- A list of "Key Focuses" using icons and background colors to highlight different areas.

### 11. Passions Section
```html
<section id="passions" class="py-20 bg-[#111111]">
```
This section describes Lakindu’s interests:
- Cards represent each passion (`Aviation`, `Music`, `Cinema`) with icons, titles, and descriptions.

### 12. Creative Work Section
```html
<section id="creative" class="py-20">
```
Highlights Lakindu's creative outlets:
- Cards showcase links to YouTube and Letterboxd profiles with a title, brief description, and "Visit Channel" links.

### 13. Connect Section
```html
<section id="connect" class="py-20 bg-[#111111]">
```
Offers links to connect on social media platforms and email. Each link uses cards with icons, hover effects, and background colors for an interactive look.

### 14. Footer
```html
<footer class="bg-[#0a0a0a] py-8">
    <div class="container mx-auto px-6 text-center text-gray-400">
        <p>© 2024 Lakindu Nisal. All rights reserved.</p>
    </div>
</footer>
```
Contains copyright information and is styled to blend with the dark theme.

### 15. `<script>`
Contains JavaScript for interactivity:
- `toggleMenu()`: Toggles the visibility of the mobile menu.
- Smooth scroll for anchor links, enhancing navigation between sections.
- GSAP animation on page load, fading in content after the welcome overlay disappears.

---
