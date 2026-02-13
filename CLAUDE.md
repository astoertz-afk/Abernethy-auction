# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Single-page static website for **"An Artful Affair"** — Abernethy Elementary School's 2026 auction fundraiser (April 18, 2026). Hosted on GitHub Pages at `auction.supportabernethy.org`.

## Architecture

- **Single file:** The entire site is one `index.html` — all CSS is inlined in `<style>`, all JS is inlined in `<script>`. No build system, no dependencies, no bundler.
- **Hosting:** GitHub Pages with custom domain via CNAME file. The main school site (`supportabernethy.org`) is on Google Sites.
- **Repo:** `astoertz-afk/Abernethy-auction` on GitHub.

## Git Workflow

- Always pull from `origin/main` before creating branches or starting work.

## Development

Open `index.html` directly in a browser. No build or install step. To preview changes, just refresh the page.

## Design System

- **Dark background (#0A0A0A)** with neon accent colors defined as CSS custom properties (`--neon-pink`, `--neon-blue`, `--neon-green`, `--neon-orange`, `--neon-violet`)
- **Typography:** Bebas Neue (display), Cormorant Garamond (serif/italic), Space Mono (body/mono) — loaded from Google Fonts
- **Paint blobs:** Decorative `div.paint` elements with organic border-radius, glow box-shadows, and floating/pulsing animations. Each section has its own set.
- **Scroll reveal:** Elements with `.reveal` class are animated in via IntersectionObserver. `.reveal-stagger` staggers children.
- **Sticky mobile CTA:** Fixed bottom bar on mobile (hidden at 768px+) that appears after scrolling past the hero.
- **Mobile-first responsive:** Breakpoints at 480px, 768px, 1024px.

## Key External Links

- Ticket purchase: BetterWorld platform (`abernethyelementaryschool.betterworld.org`)
- Volunteer signup: Konstella
- Contact: `auction@supportabernethy.org`
