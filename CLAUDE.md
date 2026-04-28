# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static HTML/CSS website for PODEM Česká republika — the official Czech distributor of PODEM crane hoists (lanové kladkostroje). The site is in Czech.

## Architecture

Single-page static site with no build system:

- [index.html](index.html) — contact/company info page; navigation links point to the main product site at `lanove-kladkostroje.cz`
- [style.css](style.css) — all styles; fixed-width layout (910px max), float-based two-column (aside + article)
- [img/](img/) — logo, header background, body background, favicon

No JavaScript, no templating, no dependencies. Deploy by copying files to a web server.

## Layout Structure

The page uses a `#wrapper` div with: `header` (logo + nav) → `section` (float: `aside` 200px left + `article` 620px right) → `footer`. The nav links to product categories on the sister site; the current page (`/`) is the contact page.
