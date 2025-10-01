# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML website template originally created by HTML Codex (the "Constra" construction template) that is being adapted for **Unigrown**, a vertical farming company. The template is being customized to replace construction-related content with vertical farming content.

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

- **HTML Pages**: All pages are in the root directory
  - `index.html` - Homepage with hero carousel, about, services, projects, team, blog, testimonials
  - `about.html`, `service.html`, `project.html`, `team.html`, `blog.html`, `testimonial.html`, `contact.html`
  - `feature.html` - Features page
  - `404.html` - Error page

- **Assets**:
  - `css/` - Compiled Bootstrap and custom styles
  - `scss/` - Bootstrap source SCSS files
  - `js/main.js` - Main JavaScript for interactions
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

### Homepage Sections (index.html)
- **Carousel**: Full-screen hero slider with zoom animation
- **About**: Two-column layout with image gallery and content
- **Features**: Three-column feature grid
- **Services**: Six service cards with hover effects
- **Counter**: Animated statistics section
- **Projects**: Recent projects grid
- **Team**: Team member cards with social links
- **Blog**: Latest blog posts
- **Testimonials**: Owl Carousel testimonial slider

### JavaScript Functionality (js/main.js)
- Spinner on page load
- Sticky navbar on scroll
- WOW.js scroll animations
- Owl Carousel for testimonials
- CounterUp for statistics
- Back to top button

## Customization for Unigrown

When adapting this template for vertical farming:
- Replace construction imagery with vertical farming images
- Update service descriptions from construction services to vertical farming solutions
- Modify project showcases to highlight vertical farming installations
- Update team member information
- Change color scheme to match Unigrown branding
- Update contact information and social media links
- Modify copy throughout to focus on sustainability, urban agriculture, and vertical farming benefits
