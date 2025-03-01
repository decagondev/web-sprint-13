# Sprint Folder Styling Guide

## Overview
This guide provides instructions for consistently styling sprint folders containing educational content using Tailwind CSS. Each sprint folder contains multiple HTML files that follow a modern, responsive design pattern.

## File Structure
Each sprint folder follows this general structure with a few variations:
```
Sprint_Folder/
├── index.html                 # Main navigation page
├── welcome.html              # Sprint welcome page
├── unit-overview.html        # Unit overview
├── tech-requirements.html    # Technical requirements
├── module-*-practice.html    # Module practice files
└── topic-specific-*.html     # Topic specific content
├── objective-01-*.html # objective files
├── objective-02-*.html
├── objective-03-*.html
```

## Required Styling Elements

### 1. Common Elements for All Files
- Tailwind CSS integration via CDN
- Responsive layout with max-width-6xl
- Color scheme:
  - Primary: #93005a
  - Secondary: #00808c
  - Background: bg-gray-50
  - Text: text-gray-900 (headings), text-gray-700 (body)
  - Links: text-blue-600 hover:text-blue-800

### 2. Page Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Page Title] - Web Unit 3 Sprint 12</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-50 min-h-screen">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
        <h1 class="text-4xl font-bold text-gray-900 mb-8 text-center">[Page Title]</h1>
        
        <div class="bg-white shadow-sm rounded-lg p-8 mb-8">
            <!-- Content goes here -->
        </div>

        <!-- Navigation -->
        <div class="flex justify-center space-x-4">
            <a href="[prev-page].html" class="inline-flex items-center px-4 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-blue-600 hover:bg-blue-700">
                ← Back to [Previous Page]
            </a>
            <a href="[next-page].html" class="inline-flex items-center px-4 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-green-600 hover:bg-green-700">
                [Next Page] →
            </a>
        </div>

        <footer class="mt-12 py-6 border-t border-gray-200 text-center text-gray-600">
            <p>Web Unit 3 Sprint 12 Curriculum - BloomTech</p>
        </footer>
    </div>
</body>
</html>
```

### 3. Common Components

#### Information Boxes
```html
<!-- Blue Info Box -->
<div class="bg-blue-50 border-l-4 border-blue-500 p-6 rounded-lg mb-8">
    <h2 class="text-2xl font-bold text-gray-900 mb-4">[Title]</h2>
    <p class="text-gray-700">[Content]</p>
</div>

<!-- Warning Box -->
<div class="bg-yellow-50 border-l-4 border-yellow-500 p-6 rounded-lg">
    <h2 class="text-2xl font-bold text-gray-900 mb-4">[Warning Title]</h2>
    <p class="text-gray-700">[Warning Content]</p>
</div>
```

#### Section Headers
```html
<div class="bg-[#00808c] text-white px-6 py-4 rounded-t-lg">
    <h2 class="text-xl font-bold">[Section Title]</h2>
</div>
<div class="border-x border-b border-gray-200 rounded-b-lg p-6">
    <!-- Section content -->
</div>
```

#### Grid Layouts
```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
    <div class="bg-gray-50 p-4 rounded-lg">
        <!-- Grid item content -->
    </div>
</div>
```

### 4. Video Integration
```html
<div class="aspect-w-16 aspect-h-9 mb-8 bg-gray-100 rounded-lg overflow-hidden">
    <iframe class="w-full h-[400px]" src="[video-url]" title="[video-title]" allow="autoplay; fullscreen" loading="lazy"></iframe>
</div>
```

### 5. Navigation Links
```html
<div class="flex justify-center space-x-4">
    <a href="[prev-page].html" class="inline-flex items-center px-4 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-blue-600 hover:bg-blue-700">
        ← [Previous]
    </a>
    <a href="[next-page].html" class="inline-flex items-center px-4 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-green-600 hover:bg-green-700">
        [Next] →
    </a>
</div>
```

## Quality Checklist
- [ ] Tailwind CSS is properly loaded
- [ ] Responsive design works on all screen sizes
- [ ] All links are working and properly styled
- [ ] Consistent spacing and padding
- [ ] Proper use of color scheme
- [ ] Semantic HTML structure
- [ ] Accessible navigation
- [ ] Proper heading hierarchy
- [ ] Consistent footer placement
- [ ] Videos are responsive

## Notes
- Use Tailwind CSS utility classes for all styling
- Maintain consistent spacing with margin and padding classes
- Use semantic HTML elements
- Ensure all interactive elements have hover states
- Keep content well-organized with appropriate headings
- Use responsive classes (sm:, md:, lg:) as needed
- Follow accessibility best practices 