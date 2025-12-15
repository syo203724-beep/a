# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-page static website about Mars colonization ("火星移住計画") written in Japanese. The site features scroll-snap navigation, CSS animations, and interactive elements.

## Development

This is a static HTML project with no build system. To view:
- Open `mars-colonization.html` directly in a browser
- Or use a local server: `python -m http.server 8000`

## Architecture

**mars-colonization.html** - Single self-contained file including:
- Embedded CSS with CSS custom properties for theming (`--mars-red`, `--accent-cyan`, etc.)
- Scroll-snap sections for chapter-based navigation
- Intersection Observer API for scroll-triggered fade-in animations
- Parallax background effects on scroll
- Interactive choice buttons with modal overlay

**External Dependencies:**
- Google Fonts (Orbitron, Noto Sans JP)
- Unsplash images (loaded via URL)

## Code Style

- CSS uses BEM-like class naming (e.g., `.section-content`, `.challenge-card`)
- Colors defined as CSS custom properties in `:root`
- Responsive breakpoints at 1024px and 768px
