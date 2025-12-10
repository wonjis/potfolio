# Portfolio Design Guidelines

This document outlines the design principles and tokens used in the `portfolio.html` specific to Wonji Seo's portfolio. Follow these rules for any future updates to maintain visual consistency.

## 1. Color Palette

The design uses a high-contrast, dark mode aesthetic.
- **Background**: `var(--bg-black)` -> `#000000` (Pure Black)
- **Text (Primary)**: `var(--text-white)` -> `#ffffff` (Pure White)
- **Text (Secondary)**: `var(--text-gray)` -> `#b8b8b8` (Light Gray for descriptions/dates)
- **Borders**: `var(--border-gray)` -> `#333333` (Dark Gray for subtle separation)
- **Accent**: `var(--accent)` -> `#ffffff` (White, used sparingly)

## 2. Typography

Two serif font families provide a premium, editorial feel.
- **Headings (Display)**: `Cormorant Garamond`
  - Weights: 300 (Light), 400 (Regular)
  - Usage: User name, section titles, project names.
  - Letter Spacing: Often increased (e.g., `0.5px`) for elegance.
- **Body Text**: `Lora`
  - Usage: Paragraphs, navigation links, buttons.
  - Line Height: `1.7` (Generous spacing for readability).

## 3. Layout & Spacing

- **Container Width**: Max `1400px`, centered (`margin: 0 auto`).
- **Section Padding**: `8rem 4rem` (Large vertical breathing room).
- **Navigation**:
  - Fixed at top (`position: fixed`).
  - Transparent black with blur: `background: rgba(0, 0, 0, 0.95)`, `backdrop-filter: blur(10px)`.
  - Height transitions on scroll.

## 4. UI Components

### Buttons & Links
- **Nav Links**:
  - Underline effect on hover (expands from left to right).
  - Opacity transition: `0.7` -> `1.0`.
- **Buttons (Load More)**:
  - Transparent background with white border.
  - Hover effect: White fill slides in from left (`transform: translateX(-100%)` -> `0`).

### Cards (Projects & Blog)
- **Style**: Minimalist, dark.
- **Border**: Thin gray border (`1px solid var(--border-gray)`).
- **Hover Effect**:
  - Main card moves up/left slightly (`translate(-2px, -2px)`).
  - A decorative "shadow" border moves down/right (`translate(10px, 10px)`).

## 5. Animations

- **Entry Animations**: Elements fade in and slide up/in.
  - `fadeInUp`: `translateY(30px)` -> `0`, `opacity` 0 -> 1.
  - `fadeInLeft` / `fadeInRight`: `translateX` shift.
- **Durations**: Typically `0.8s` with ease-out curves.
- **Staggering**: Child elements (like nav links) have delay offsets (`0.1s`, `0.2s`, etc.).

## 6. Iconography

- **Social Icons**: Simple text characters (e.g., "𝕏", "in") or SVG paths.
- **Style**: Minimal, monochromatic (white).
