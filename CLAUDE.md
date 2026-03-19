# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static personal portfolio site for "CheshirePleb" — built on the **Solid State** template by HTML5 UP. No build tools, package manager, or test framework. Pages are plain HTML served directly.

## Development

Open any `.html` file in a browser to preview. No build step or dev server is required.

## Architecture

- **Pages**: `index.html` (home/projects), `about.html` (bio), `photos.html`, `generic.html`, `elements.html` (template reference)
- **Styling**: `assets/sass/` contains SASS source files; `assets/css/main.css` is the compiled stylesheet. `noscript.css` provides fallback styles.
- **JS**: jQuery-based — `assets/js/main.js` is the primary custom script; other JS files are vendor libraries (jQuery, Scrollex, breakpoints, browser detection).
- **Images**: `images/` — includes project screenshots and template placeholder images.
- **Navigation menu** is duplicated in each HTML file (no templating system) — changes to nav must be applied to every page.

## Key Details

- Licensed under Creative Commons Attribution 3.0 (HTML5 UP template license).
- The nav menu links to an external Gallery app hosted on Vercel. Note: `index.html` and `about.html` currently point to different Gallery URLs — this is an existing inconsistency.
- Footer contact sections are also duplicated across pages with slight differences.
