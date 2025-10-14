# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based blog called "tales of existance" hosted at talesofexistence.com. The site uses the "moving" theme and includes custom analytics integration via Plausible.

## Development Commands

### Local Development
```bash
bundle exec jekyll serve
```
This starts a local development server with auto-regeneration on file changes. Note: Changes to `_config.yml` require a server restart.

### Install Dependencies
```bash
bundle install
```

## Architecture

### Site Structure
- **_posts/**: Blog posts in Markdown format, named with pattern `YYYY-MM-DD-title.markdown`
- **_config.yml**: Main site configuration including title, description, theme, plugins, and analytics
- **index.markdown**: Homepage with `layout: home`
- **about.markdown**: About page
- **404.html**: Custom 404 error page

### Configuration Details
- Theme: `moving`
- Plugins: `jekyll-feed`, `jekyll-analytics`
- Analytics: Custom Plausible instance at plausible.purplebird.xyz
- Jekyll version: ~> 4.0.0

### Blog Post Format
Posts must include front matter with:
- `layout: post`
- `title: "Post Title"`
- `date: YYYY-MM-DD HH:MM:SS +ZZZZ`
- `categories: category names`

File naming convention: `YYYY-MM-DD-title.markdown` in `_posts/` directory.

### Custom Analytics
The site uses a self-hosted Plausible Analytics instance. Configuration is in `_config.yml` under `jekyll_analytics.Plausible` with custom domain and source URL.
