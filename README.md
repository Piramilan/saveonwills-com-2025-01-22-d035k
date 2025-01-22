# SaveonWills.com Landing Page Maintenance Guide

This guide will help you maintain and customize the SaveonWills.com landing page. Whether you're new to HTML and CSS or just getting started, we'll walk you through the essential updates you might need to make.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the logo and navigation menu. To update the logo text:

```html
<!-- Find this section near the top -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    SaveonWills.com  <!-- Change this text to update the logo -->
</a>
```

### Hero Section Text
To update the main headline and subheading:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    Protect Your Wishes, Protect Your Loved Ones—Start Your Will Now  <!-- Main headline -->
</h1>
<p class="text-xl text-gray-600 mb-12 leading-relaxed">
    Create your will online with expert guidance and support.  <!-- Subheading -->
</p>
```

### Tailwind CSS Classes Explained
Common classes used throughout the page:

- Text sizes: `text-xl`, `text-2xl`, `text-3xl`, etc.
- Colors: `text-gray-600`, `bg-blue-600`
- Spacing: `px-6` (padding left/right), `py-4` (padding top/bottom), `mb-8` (margin bottom)
- Responsive design: `md:text-5xl` (applies at medium screens and up)

To modify a style, simply change the corresponding class value. For example:
```html
<!-- Original -->
<button class="bg-blue-600 text-white px-6 py-2">

<!-- Modified for larger padding -->
<button class="bg-blue-600 text-white px-8 py-4">
```

## Fixing Broken Links

### Navigation Menu Links
The main navigation menu contains these links:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update a link:
1. Locate the `href` attribute
2. Replace the value with your desired URL
3. For internal sections, use `#section-id`
4. For external links, use the full URL: `https://example.com`

Example:
```html
<!-- Original internal link -->
<a href="#features">Features</a>

<!-- Updated external link -->
<a href="https://saveonwills.com/features">Features</a>
```

## Linking Privacy and Terms Pages

### Footer Links Section
Locate the legal section in the footer:

```html
<div>
    <h4 class="text-white text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Replace the `#` with the correct path
2. Ensure the files exist in your project

Example:
```html
<!-- Updated privacy and terms links -->
<li><a href="/privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="/terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Layout**
   - Check that you haven't removed any essential Tailwind classes
   - Verify all closing tags are present
   - Ensure the Tailwind CDN link is working:
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```

2. **Links Not Working**
   - Verify file paths are correct
   - Check for typos in `href` attributes
   - Ensure IDs match exactly for internal links

3. **Images Not Displaying**
   - Confirm image paths are correct
   - Check file extensions match exactly
   - Verify images are in the correct directory

### Need Help?
If you encounter issues:
1. Check the browser's developer tools (F12) for errors
2. Verify all files are in the correct locations
3. Double-check your changes against the original code
4. Contact support at help@saveonwills.com

Remember to always backup your files before making changes!