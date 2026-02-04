# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A personal portfolio website for Pierre-Alexandre Dupuy (Senior Frontend Engineer / Engineering Manager / AI Engineer). The site features a technical/industrial aesthetic with dark/light mode support.

## Architecture

Astro 5.17 static site with Tailwind CSS v4:
- `src/pages/index.astro` - Main portfolio page
- `src/layouts/Layout.astro` - Base layout with fonts, dark mode, decorative elements
- `src/components/` - Modular components (Header, Hero, DataMatrix, ClaudeBridge, Footer)
- `src/styles/global.css` - Tailwind theme and custom CSS classes

## Commands

```bash
pnpm dev          # Start dev server (localhost:4321)
pnpm build        # Build static site to dist/
pnpm preview      # Preview production build
```

## Deployment

GitHub Pages via GitHub Actions (`.github/workflows/deploy.yml`). Auto-deploys on push to `main`.
Site URL: https://padupuy.github.io/portfolio

## Design System

- **Primary color**: `#FF4D00` (orange)
- **Fonts**: JetBrains Mono (monospace), Inter (display headings)
- **Theme**: Industrial/technical aesthetic with grid backgrounds, scanlines, and technical labels
- **Dark mode**: Class-based switching (`html.dark` / `html.light`)
