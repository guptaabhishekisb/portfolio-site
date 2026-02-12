# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static portfolio/resume website for Abhishek Gupta, Director of Product at Expedia Group. The entire site is a single-file HTML document with embedded CSS and JavaScript.

## Running the Site

Open `resume.html` directly in a web browser:
```bash
open resume.html
```

Or serve it locally with a simple HTTP server:
```bash
python3 -m http.server 8000
# Then visit http://localhost:8000/resume.html
```

## Architecture

**Single-file architecture**: All HTML structure, CSS styling, and JavaScript functionality are embedded in `resume.html` (1,283 lines).

**Key sections** (in order):
- Navigation (fixed header with responsive hamburger menu)
- Hero (name, title, summary with avatar and CTAs)
- Stats bar (animated statistics)
- Experience timeline (Expedia, Google, earlier roles)
- Skills grid (6 core competencies)
- Education (ISB, Engineering degree, languages)
- Leadership & Speaking (4 highlight cards)
- Contact form (LinkedIn, location, message form)
- Footer

**CSS approach**:
- CSS variables defined in `:root` for theming (colors, shadows, borders)
- Mobile-first responsive design with `@media (max-width: 768px)`
- Scroll-triggered fade-in animations using IntersectionObserver
- Print styles for resume printing

**JavaScript features**:
- Smooth scroll navigation with active link highlighting
- Navbar scroll shadow effect
- Mobile hamburger menu toggle
- Intersection Observer for scroll-reveal animations
- Animated stat counters
- Contact form submission handling (simulated)

## Making Changes

When editing the site:
- **Styling**: Modify CSS in the `<style>` block (lines 7-822) - prefer using existing CSS variables for colors
- **Content**: Update HTML sections directly (lines 824-1179)
- **Behavior**: Modify JavaScript in the `<script>` block (lines 1181-1280)
- **Colors**: Primary branding uses `--accent: #2c7be5` (blue) and `--primary: #1a2a3a` (dark navy)

## External Links

The site links to:
- LinkedIn: `https://www.linkedin.com/in/guptaabhishekisb/`
- Contact email: `abhishek@example.com` (placeholder)
