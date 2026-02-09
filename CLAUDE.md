# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal portfolio and blog website for Sichen Li, built using the dev-portfolio-blog theme. The site includes sections for education, work experience, publications, skills and honors, and a blog for project showcases.

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Serve the site locally with live reload
bundle exec jekyll serve

# Build the site for production
bundle exec jekyll build

# Clean build artifacts
bundle exec jekyll clean
```

### Testing
The site is deployed via GitHub Pages, so test locally before committing changes.

## Architecture

### Directory Structure
- `_config.yml` - Main Jekyll configuration with plugins, pagination, minification settings
- `_layouts/` - HTML templates for different page types
  - `default.html` - Base template with header, analytics, and theme selector
  - `post.html` - Blog post template with categories and Disqus comments
  - `home.html`, `page.html`, `list.html` - Various page layouts
  - `workexperience.html`, `description.html` - Custom layouts for portfolio sections
- `_includes/` - Reusable HTML components
  - `navigation.html` - Site navigation menu
  - `themeSelector.html` - Dark mode toggle
  - `analytics.html` - Google Analytics integration
  - `disqus_comments.html` - Comment system
  - `share_buttons.html` - Social media sharing
- `_posts/` - Blog posts in markdown format (yyyy-mm-dd-title.md)
- `_sass/` - Stylesheets
- `assets/` - Static assets (JS, CSS, images)
- `figure/` - Images for blog posts

### Key Features
- **Dark Mode**: Theme toggle via `themeSelector.html` and `theme.js`
- **Google Analytics**: Integrated via `_includes/analytics.html` and gtag in default layout
- **Disqus Comments**: Configurable per-post via YAML front matter
- **Jekyll Pagination**: Posts paginated at 10 per page
- **Jekyll Minifier**: Automatic minification of HTML, CSS, JS
- **SEO Optimization**: Using jekyll-seo-tag plugin
- **Emoji Support**: Via jemoji plugin

### Content Management
- Main pages: `index.md`, `about.md`, `education.md`, `publication.md`, `skillsandhonors.md`, `workexperience.md`, `categories.md`
- PDFs: `Resume.pdf`, `Recommendation.pdf`, `Azure_All.pdf`
- Blog posts use categories for organization (e.g., "Banking Credit Risk Project")

### Blog Post Format
```yaml
---
layout: post
comments: [true|false]
title: Your Post Title
categories: [category1, category2]
---
Post content here.
```

### Configuration Notes
- Ruby version: 3.2.2
- Google Analytics ID configured in `_config.yml` (line 151)
- Disqus shortname configured in `_config.yml` (line 157)
- Resume URL configurable via `resume_url` in `_config.yml`

## Important Details
- Images in blog posts are referenced relative to the `figure/` directory
- The site uses Jekyll Assets plugin for asset management with autoprefixer
- Navigation structure is maintained in `_includes/navigation.html`
- Theme switching JavaScript is in `assets/js/theme.js`
