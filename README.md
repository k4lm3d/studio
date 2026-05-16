# studio

[![Hosted on GitHub: k4lm3d/studio](https://img.shields.io/badge/k4lm3d-studio-teal?style=for-the-badge&logo=github)](https://github.com/k4lm3d/studio)
[![Deployed on Cloudflare Pages](https://img.shields.io/badge/demo-zap--studio-orange?style=for-the-badge&logo=cloudflare)](https://zap-studio.pages.dev)
[![Prompted with ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)](https://chatgpt.com)
[![Coded with Google AI Studio / Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://aistudio.google.com)

**Studio** is a modern SaaS-style landing page inspired by the design, structure, and overall user experience of [WeConnectPH Studio](https://weconnectph.com/studio).

## Features

- Modern UI with glassmorphism and subtle gradients
- Fully responsive (mobile-first)
- Smooth scrolling and micro animations
- Sticky transparent navbar with blur effect
- Rounded cards, soft shadows, clean spacing
- Fast-loading static frontend only (no backend needed)

## Layout Structure

1. Hero Section

    - Large bold heading
    - Small subtitle text
    - CTA buttons (“Download”, “View Releases”)
    - Product/mockup preview on the right side
    - Animated glowing background
    - Floating UI effects

2. Feature Grid

    - 3–6 modern feature cards
    - Each card with icon, title, description
    - Hover animations
    - Minimal neon accents

3. Releases Section

    - Modern release cards
    - Version number
    - Release date
    - Download button
    - Changelog link
    - OS badges (Windows/Linux/macOS)

4. Changelog Section

    - Timeline-style UI
    - Compact update cards
    - Modern typography
    - GitHub-style formatting

5. Roadmap Section

    - Public roadmap layout
    - Status badges:
        - Planned
        - In Progress
        - Completed
    - Clean kanban-inspired design

6. Footer

    - Minimal footer
    - Social links
    - GitHub link
    - Copyright text
    - Dark gradient background

## Style Guide

- Typography:

  - Inter font
  - Large bold headings
  - Muted secondary text

- Colors:

  - Background: #0B0F19
  - Cards: rgba(255,255,255,0.05)

- Accent: blue/purple gradient

- Text: white with muted gray

- Animations:

  - Hover lift effects
  - Glow animations
  - Fade-in on scroll

## Tech Stack

+ Pure HTML
+ TailwindCSS
+ Vanilla JavaScript
+ ~~Lucide Icons~~
+ Alpine.JS
+ Feather Icons

## Bonus Features

- ~~Dark/light mode toggle~~
- Animated background grid
- ~~GitHub releases auto-fetch support~~
- SEO meta tags
- Open Graph support
- Smooth page transitions

### Key Design Decisions & Implementation Details

1.  **Glassmorphism Engine:** Used `backdrop-blur-md` and `bg-white/5` combined with a 1px `border-white/10`. This creates the layered "frosted glass" effect seen on premium SaaS sites like Vercel and Raycast.

2.  **Typography:** Implemented the **Inter** font family with a negative `tracking-tight` on headings and `tracking-widest` on small labels to give it a modern, architectural feel.

3.  **Background Grid:** A custom CSS `radial-gradient` creates a subtle dot grid that stays fixed as you scroll, adding depth to the dark mode.

4.  **Floating Mockup:** The Hero section includes a CSS-animated `animate-float` mockup. It uses a "blurred glow" background (an indigo/purple blob) that mimics the lighting used by high-end design agencies.

5.  **Roadmap Layout:** Inspired by Kanban boards, the roadmap uses status-specific colors (Gray for planned, Indigo for in-progress, Green for completed) with a progress bar for the "active" task.

6.  **Micro-Interactions:** 
    *   **Smooth Scroll:** native `scroll-smooth` class.
    *   **Scroll Reveal:** A simple `IntersectionObserver` script fades in sections as you scroll.
    *   **Hover Lifts:** Feature cards use `hover:-translate-y-2` for a premium interactive feel.

7.  **Responsive:** The layout shifts from a 2-column hero to a stacked layout on mobile seamlessly using Tailwind's `lg:grid-cols-2`.

### How to use

1. To customize the accent color, simply change the `accent-primary` and `accent-secondary` values in the Tailwind config script at the top.

.
