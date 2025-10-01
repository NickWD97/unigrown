# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **single-page static HTML website** originally created by HTML Codex (the "Constra" construction template) that is being adapted for **Unigrown**, a vertical farming company. The template has been converted from a multi-page layout to a single-page application with smooth scroll navigation.

## Technology Stack

- **Frontend Framework**: Bootstrap 5
- **JavaScript Libraries**:
  - jQuery 3.6.4
  - WOW.js (scroll animations)
  - Owl Carousel (testimonial carousel)
  - CounterUp (animated counters)
  - Waypoints (scroll tracking)
  - Lightbox (image galleries)
- **CSS**: Custom styles in `css/style.css` with Bootstrap variables
- **Fonts**: Playfair Display and Roboto from Google Fonts
- **Icons**: Font Awesome 5 and Bootstrap Icons

## Project Structure

- **Single Page Application**:
  - `index.html` - Complete single-page website with all sections:
    - Hero carousel
    - About (#about)
    - Features (#features)
    - Services (#services)
    - Counter/Statistics
    - Projects (#projects)
    - Team (#team)
    - Blog (#blog)
    - Testimonials (#testimonials)
    - Contact (#contact)
    - Footer

- **Assets**:
  - `css/` - Compiled Bootstrap and custom styles
  - `scss/` - Bootstrap source SCSS files
  - `js/main.js` - Main JavaScript with smooth scroll navigation
  - `img/` - Images directory
  - `lib/` - Third-party libraries (owl carousel, wow, easing, waypoints, counterup, animate.css)

## Development Workflow

This is a **static website** with no build process. Changes are made directly to HTML, CSS, and JavaScript files.

### Viewing the Site

Open HTML files directly in a browser or use a local web server:
```bash
python -m http.server 8000
# OR
python3 -m http.server 8000
```

Then navigate to `http://localhost:8000`

### Making Style Changes

- Edit `css/style.css` for custom styles
- Bootstrap customization requires editing SCSS files in `scss/bootstrap/` and recompiling

### Color Scheme

The template uses Bootstrap CSS variables:
- Primary color: Blue (`--bs-primary`)
- Secondary color: Orange (`--bs-secondary`)
- These will need to be updated to match Unigrown's vertical farming brand identity

## Key Components

### Page Sections (index.html)
All sections are accessible via smooth scroll anchor navigation:

- **Carousel**: Full-screen hero slider with zoom animation
- **About (#about)**: Two-column layout with image gallery and content
- **Features (#features)**: Three-column feature grid
- **Services (#services)**: Six service cards with hover effects
- **Counter**: Animated statistics section
- **Projects (#projects)**: Recent projects grid
- **Team (#team)**: Team member cards with social links
- **Blog (#blog)**: Latest blog posts
- **Testimonials (#testimonials)**: Owl Carousel testimonial slider
- **Contact (#contact)**: Contact form, Google Maps, and contact info cards

### Navigation
- Single-page navigation using anchor links
- Smooth scroll to sections with 100px offset for sticky navbar
- Active nav link highlighting based on scroll position
- Footer links also use anchor navigation

### JavaScript Functionality (js/main.js)
- Spinner on page load
- Sticky navbar on scroll
- WOW.js scroll animations
- Owl Carousel for testimonials
- CounterUp for statistics
- Back to top button
- Smooth scroll navigation for anchor links
- Automatic active nav link updates on scroll

## Customization for Unigrown

When adapting this template for vertical farming:
- Replace construction imagery with vertical farming images
- Update service descriptions from construction services to vertical farming solutions
- Modify project showcases to highlight vertical farming installations
- Update team member information
- Change color scheme to match Unigrown branding
- Update contact information and social media links
- Modify copy throughout to focus on sustainability, urban agriculture, and vertical farming benefits
