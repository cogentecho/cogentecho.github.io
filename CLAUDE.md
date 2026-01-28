# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the public website for Cogent Echo, hosted on GitHub Pages at cogentecho.ai. It's a static site with no build process.

## Architecture

- **index.html** - Main landing page with n8n webhook integration for agent communication
- **CNAME** - Custom domain configuration pointing to cogentecho.ai
- Static HTML/CSS/JS only - no framework, no build step

## Development

To test locally, serve the files with any static server:
```bash
python -m http.server 8000
# or
npx serve .
```

Changes pushed to `main` automatically deploy via GitHub Pages.

## External Integration

The site connects to an n8n workflow at `https://cogentecho.app.n8n.cloud/webhook/cogentecho.ai` for backend agent functionality.
