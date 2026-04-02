# CLAUDE.md — MXE Media Website

## Project Overview

Static HTML website for MXE Media, a video production company. Three standalone HTML pages with no build process, no package manager, and no framework — pure HTML, CSS, and vanilla JS.

## File Map

### Pages (all UI lives here)

| File | Purpose |
|------|---------|
| `index.html` | Home page — nav, hero, descriptor band, work grid, values, testimonial, map, trusted-by scroller, contact CTA, footer |
| `production.html` | Production services page — hero, equipment band, how-we-work, services grid, photo strip |
| `contact.html` | Contact page — hero, contact form, contact info, location band, footer |

### Images & Assets (all at root level)

| File | Used In |
|------|---------|
| `mxe_website_hero_photo.jpg` | `index.html` hero |
| `mxe_website_hero_photo_darker.jpg` | `production.html` hero |
| `MXEFILMS_Work Locations.png` | `index.html` map section |
| `M and L Interview Wide.png` | `production.html` interview photo |
| `Photo (1).jpg` – `Photo (27).jpg` | `production.html` photo strip grid |

## Styles & Config

- **No external CSS files.** All styles are in `<style>` blocks inside each HTML file's `<head>`.
- **CSS variables** (colors, fonts) are declared at the top of each `<style>` block — edit these to change the global look.
- Key variables:
  - `--amber: #c8794a` — accent color
  - `--font-display: 'Cormorant Garamond'` — headings
  - `--font-body: 'Outfit'` — body text
- **Responsive breakpoints:** `max-width: 900px` and `max-width: 600px` near the bottom of each `<style>` block.
- **No config files** (no package.json, tailwind.config.js, etc.).

## Key CSS Classes (for layout changes)

| Class | What It Controls |
|-------|-----------------|
| `.nav-inner`, `.nav-links` | Navigation bar |
| `.hero`, `.prod-hero`, `.contact-hero` | Page hero sections |
| `.work-grid` | 4-column portfolio grid (index) |
| `.values-grid` | 3-column values cards (index) |
| `.services-grid` | 2-column services grid (production) |
| `.photo-strip-grid` | 9-column photo gallery (production) |
| `.contact-form` | Contact form layout |
| `.fade-up` | Scroll-triggered fade-in animation |
| `.scrollTrusted` | Infinite horizontal brand scroller |

## Working Instructions

- **Only read files directly needed for the task.** Don't scan all pages to change one section.
- **Do not refactor, reformat, or clean up code** that wasn't part of the request.
- **Keep responses concise** — confirm what was changed and where, nothing more.
- **Do not install packages or add dependencies** without asking first.
- **No build step needed** — edits to HTML files take effect immediately in the browser.
- When adding images, place them at the root level alongside existing assets.
- Navigation HTML is duplicated across all three files — if changing nav, update all three.
