# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static GitHub Pages website for the Jonah Lomu Rugby Mod (JLR) - a mod for the classic rugby video game. Hosted at jlr.nz.

## Development

No build process required. This is a pure static HTML/CSS/JS site.

**Local preview**: Open any HTML file directly in a browser, or use a local server:
```bash
python -m http.server 8000
```

## Architecture

- **Bootstrap 5.3.3** loaded from CDN, with custom theme overrides in `assets/css/bs-theme-overrides.css`
- **Color scheme**: Primary (#000139 dark navy), Secondary (#ff8000 orange)
- **Fonts**: Work Sans (body), Raleway (headings) via Google Fonts
- **Single JS file** (`assets/js/startup-modern.js`) handles navbar shrink-on-scroll behavior
- **Google Analytics** tracking included in all pages

## File Structure

```
├── index.html        # Homepage
├── download.html     # Download page
├── history.html      # Release notes/version history
├── support.html      # Support documentation
├── contact.html      # Contact form
├── sitemap.xml       # SEO sitemap
├── CNAME             # Custom domain (jlr.nz)
└── assets/
    ├── bootstrap/css/  # Bootstrap CSS
    ├── css/            # Custom styles
    ├── js/             # Custom JavaScript
    └── img/            # Images (prefer WebP format)
```

## Conventions

- Use WebP format for new images where possible (existing images are mixed PNG/WebP)
- All pages share the same navbar and footer structure
- Content uses Bootstrap utility classes for layout and spacing
