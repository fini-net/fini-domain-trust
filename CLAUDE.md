# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Hugo-based static website for the FINI Domain Trust project, which maintains domain ownership to prevent spam and abuse. The site is published to GitHub Pages via GitHub Actions.

## Architecture

- **Hugo Site Root**: `trust/` directory contains all Hugo configuration and content
- **Theme**: Uses the Ananke theme as a git submodule at `trust/themes/ananke`
- **Published Output**: `trust/public/` directory (symlinked as `html` at repo root)
- **GitHub Pages**: Automated deployment via `.github/workflows/github-pages.yml` which pushes `trust/public` to the `gh-pages` branch on every push to `main`

## Common Commands

All Hugo commands must be run from the `trust/` directory:

```bash
cd trust

# Build the site (generates static files in public/)
hugo

# Run development server with live reload
hugo server

# Run development server with drafts visible
hugo server -D

# Clean build artifacts
rm -rf public/ resources/
```

## Content Structure

- **Main Content**: `trust/content/_index.md` is the homepage
- **Configuration**: `trust/hugo.toml` contains site configuration and social links
- **Static Assets**: `trust/static/` for images and other static files
- **Archetypes**: `trust/archetypes/default.md` for content templates

## Git Submodules

The Ananke theme is included as a git submodule. When cloning fresh or after theme updates:

```bash
git submodule update --init --recursive
```

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to `main`. The workflow builds Hugo if needed (though currently commented out) and publishes `trust/public/` to the `gh-pages` branch.
