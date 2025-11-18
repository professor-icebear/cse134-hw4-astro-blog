# Tech Blog - Astro Static Site

A modern, high-performance blog built with Astro, featuring smooth View Transitions and minimal JavaScript.

## Features

- 🚀 **Blazing Fast**: Static site generation with zero JavaScript by default
- 🎨 **Modern Design**: Beautiful, responsive UI with gradient accents
- 🔄 **View Transitions**: Smooth page transitions using the View Transition API
- 📝 **Markdown Blog Posts**: Easy content management with Markdown
- 🏷️ **Tag System**: Organize posts with tags and filter by category
- 📱 **Responsive**: Works perfectly on all devices
- ♿ **Accessible**: Built with accessibility in mind

## Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── BlogCard.astro      # Reusable blog post card component
│   │   ├── Footer.astro        # Site footer component
│   │   ├── Header.astro        # Navigation header with View Transitions
│   │   └── TagList.astro       # Tag filtering component
│   ├── content/
│   │   └── blog/               # Markdown blog posts
│   ├── layouts/
│   │   ├── BaseLayout.astro    # Base layout for all pages
│   │   └── BlogLayout.astro    # Specialized layout for blog posts
│   ├── pages/
│   │   ├── index.astro        # Homepage
│   │   ├── about.astro        # About page
│   │   └── blog/
│   │       ├── index.astro    # Blog listing page
│   │       ├── [...slug].astro # Dynamic blog post pages
│   │       └── tag/
│   │           └── [tag].astro # Tag filtering page
│   └── styles/
│       └── global.css         # Global styles
└── package.json
```

## Components & Layouts

### Reusable Components

- **Header.astro**: Navigation header with View Transition scoping
- **Footer.astro**: Site footer with links
- **BlogCard.astro**: Displays blog post previews with metadata
- **TagList.astro**: Tag filtering interface

### Layouts

- **BaseLayout.astro**: Base layout used across all pages
- **BlogLayout.astro**: Specialized layout for blog posts with metadata display

## View Transitions

This site implements the View Transition API for smooth page transitions:

- **Header Transitions**: Navigation header transitions smoothly between pages
- **Content Transitions**: Blog content animates when navigating between posts
- **Tag Transitions**: Tag filters transition smoothly

View Transitions are enabled via Astro's built-in `ViewTransitions` component in the Header.

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

4. Preview production build:
```bash
npm run preview
```

## Adding Blog Posts

Create a new markdown file in `src/content/blog/` with the following frontmatter:

```markdown
---
title: "Your Post Title"
description: "A brief description of your post"
date: 2024-01-15
tags: ["Tag1", "Tag2"]
readingTime: 5
---

Your post content here...
```

## Browser Support

- Modern browsers with View Transition API support (Chrome 111+, Safari 18+)
- Gracefully degrades in browsers without View Transition support

## Performance

This site is optimized for performance:

- Static HTML generation
- Minimal JavaScript (only for View Transitions)
- Optimized CSS
- Fast page loads
- Excellent Core Web Vitals scores

## License

This project is created for educational purposes as part of CSE 134B coursework.

