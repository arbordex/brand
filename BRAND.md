# Arbor DEX Brand Guidelines

**Organization:** Arbor DEX  
**Repository:** `arbordex/brand` (GitHub)  
**Version:** 3.0 (Consolidated)  
**Last Updated:** December 2025  
**Status:** Official, Single-Source Brand System

---

## Quick Links

- [Brand Essence](#brand-essence)
- [Vision & Core Values](#vision--core-values)
- [Visual Identity](#visual-identity)
- [Colors](#colors)
- [Typography](#typography)
- [Voice & Tone](#voice--tone)
- [Logo Usage](#logo-usage)
- [Resources](#resources)

---

## Brand Essence

**Arbor DEX** is a professional, modular DEX application built to explore DeFi architecture while maintaining code clarity and welcoming contributors.

We are not a teaching platform. We are a real DeFi application where concepts are implemented thoughtfully, code is maintainable, and the structure is intentional enough that others can read, understand, and build on it.

**Elevator Pitch:**  
Arbor DEX is a modular DEX server - built with love, easy to understand, and open to the community.

---

## Vision & Core Values

### Vision

To build a DEX backend that is simultaneously:

- **Real** – A genuine DeFi application, not a tutorial.
- **Clear** – Code and architecture that can be read and extended.
- **Community-driven** – A codebase that welcomes contributors and learners.

### Core Values

| Value | Description |
|-------|-------------|
| **Clarity** | Code, design, and messaging should be easy to understand. No obfuscation. |
| **Quality** | Professional standards applied to structure, testing, and security. |
| **Accessibility** | Welcoming to contributors, learners, and those who want to build further. |
| **Modernity** | Tech-forward practices (TypeScript, ESLint, environment separation). |
| **Warmth** | Approachable, human-centered design that feels collaborative, not cold. |
| **Honesty** | No hype, no false promises. Real implementation, real learning. |

---

## Visual Identity

### Logo System

The **Arbordex tree mark** is the visual cornerstone of the brand:

- **Tree trunk** represents the protocol core.
- **Branches** represent liquidity routes and AMM connections.
- **Canopy circles** represent pools and markets.
- **Node dots** represent assets and participants.

**Design Language:**

- Soft, rounded shapes (warm and inviting).
- Organic curves (growth and flow).
- Scalable at any size (from favicon to billboard).
- Works on light, dark, and colored backgrounds.

### Logo Variants

| Variant | Use Case | Files | Color |
|---------|----------|-------|-------|
| **Primary** | Web, social, apps, marketing | `arbordex-logo-cyan.svg` | `#00FFFF` |
| **Black** | Print, business cards, light backgrounds | `arbordex-logo-black.svg` | `#000000` |
| **White** | Dark mode, dark backgrounds | `arbordex-logo-white.svg` | `#FFFFFF` |
| **Icon Only** | Favicon, avatar, small UI | `arbordex-mark.svg` | Varies |
| **Full Lockup** | Headers, docs, presentations | `arbordex-full-lockup.svg` | Varies |

---

## Colors

### Palette

| Color | Hex | RGB | Use |
|-------|-----|-----|-----|
| **Arbordex Cyan** | `#00FFFF` | 0, 255, 255 | Primary accent, logo, CTA |
| **Dark Teal** | `#004B57` | 0, 75, 87 | Hero backgrounds, dark mode |
| **Ink Black** | `#05070A` | 5, 7, 10 | Text on light backgrounds |
| **Clean White** | `#FFFFFF` | 255, 255, 255 | Text on dark, light backgrounds |
| **Light Teal** | `#55F2E3` | 85, 242, 227 | Secondary elements, hover states |
| **Light Gray** | `#F8F9FA` | 248, 249, 250 | Accessibility, light backgrounds |
| **Soft Gray** | `#E8E8E8` | 232, 232, 232 | Breathing room, dividers |
| **Medium Slate** | `#1A1F3A` | 26, 31, 58 | Text on colored backgrounds |

### Usage Guidelines

**On Light Backgrounds:**

- Logo: Cyan (`#00FFFF`)
- Text: Ink Black (`#05070A`)
- Accents: Cyan or Light Teal

**On Dark Backgrounds:**

- Logo: Cyan (`#00FFFF`) or Light Teal (`#55F2E3`)
- Text: Clean White (`#FFFFFF`)
- Accents: Light Teal (`#55F2E3`)

**Monochrome (Print/Single-Color):**

- All elements in 100% Black or 100% White only.

### CSS Variables

```css
:root {
  /* Primary Colors */
  --color-cyan: #00FFFF;
  --color-teal-dark: #004B57;
  --color-black: #05070A;
  --color-white: #FFFFFF;

  /* Secondary Colors */
  --color-teal-light: #55F2E3;
  --color-gray-light: #F8F9FA;
  --color-gray-soft: #E8E8E8;
  --color-slate: #1A1F3A;

  /* Light Mode */
  --bg-primary: var(--color-white);
  --bg-secondary: var(--color-gray-light);
  --text-primary: var(--color-black);
  --text-secondary: var(--color-slate);

  /* Dark Mode */
  --bg-primary-dark: var(--color-teal-dark);
  --bg-secondary-dark: var(--color-slate);
  --text-primary-dark: var(--color-white);
  --text-secondary-dark: var(--color-gray-light);
}

@media (prefers-color-scheme: dark) {
  body {
    background-color: var(--bg-primary-dark);
    color: var(--text-primary-dark);
  }
}
```

---

## Typography

### Font Families

| Font | Use | Source |
|------|-----|--------|
| **Inter** (400, 500, 600, 700) | UI, web, marketing | [Google Fonts](https://fonts.google.com/specimen/Inter) |
| **IBM Plex Mono** (400, 600) | Code, technical content | [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Mono) |

**CSS Stack (Inter):**

```css
font-family: "Inter", system-ui, -apple-system, BlinkMacSystemFont, 
             "Segoe UI", sans-serif;
```

**CSS Stack (Mono):**

```css
font-family: "IBM Plex Mono", ui-monospace, SFMono-Regular, Menlo, Monaco,
             "Liberation Mono", "Courier New", monospace;
```

### Text Hierarchy

| Level | Font | Weight | Size | Line Height | Use |
|-------|------|--------|------|-------------|-----|
| **H1** | Inter | Bold (700) | 32–40px | 1.2 | Page titles, hero headlines |
| **H2** | Inter | SemiBold (600) | 24–28px | 1.3 | Section headings |
| **H3** | Inter | SemiBold (600) | 18–22px | 1.4 | Subsection headings |
| **H4** | Inter | Medium (500) | 16–18px | 1.5 | Mini headings, cards |
| **Body** | Inter | Regular (400) | 14–16px | 1.6 | Paragraph text, descriptions |
| **Small** | Inter | Regular (400) | 12–14px | 1.5 | Labels, captions, metadata |
| **Code** | IBM Plex Mono | Regular (400) | 12–14px | 1.5 | Code blocks, inline code |

### Text Colors

**Light Mode:**

- Headings: Ink Black (`#05070A`)
- Body: Medium Slate (`#1A1F3A`)
- Links: Cyan (`#00FFFF`)

**Dark Mode:**

- Headings: Clean White (`#FFFFFF`)
- Body: Light Gray (`#F8F9FA`)
- Links: Light Teal (`#55F2E3`)

---

## Voice & Tone

### Brand Voice

- **Friendly** – Approachable and collaborative, not corporate.
- **Honest** – Real, transparent, no hype or false promises.
- **Clear** – Direct and understandable, minimal jargon.
- **Professional** – Competent and intentional, not amateur.
- **Warm** – Human-centered, inviting, not cold or dismissive.

### Examples

**✅ Good (Arbordex Voice):**

- "Build, explore, and understand DeFi from the ground up."
- "Code is meant to be read and modified."
- "We're learning DeFi together - and we want you along for the ride."
- "Transparency by default. No gatekeeping."

**❌ Avoid:**

- "Enterprise-grade blockchain infrastructure."
- "Revolutionizing decentralized markets."
- "For advanced traders only."
- "Cutting-edge AI-powered DeFi solutions." (Hype and buzzwords)

### Copy Guidelines

- Use contractions ("we're", "don't") for conversational tone.
- Avoid jargon; explain technical terms when necessary.
- Write in active voice ("We built X" not "X was built by us").
- Keep paragraphs short and scannable.
- Lead with benefit or insight, not the mechanism.

---

## Logo Usage

### Sizing

**Digital:**

- 16×16px (favicon)
- 32×32px (small UI icon)
- 64×64px (medium app icon)
- 128×128px (avatar, social)
- 256–512px (web, large)

**Print:**

- 0.5"×0.5" (small, email signature)
- 0.75"×0.75" (medium, business card)
- 1.0"+ (large, stationery)
- 2.0"+ (extra-large, posters)

### Placement

- **Website header:** Logo + wordmark, left-aligned or centered (48–64px)
- **Social avatar:** Icon only (128–512px depending on platform)
- **Documentation:** Small mark next to headings (24–48px)
- **Favicon:** Icon mark (16px or 32px)
- **Business cards:** Full lockup (0.75"×0.75")
- **Hero section:** Large centered mark (128px+)

### Clear Space

Maintain **at least 8px** of breathing room around the logo on all sides.

```text
┌────────────────────┐
│  ░░░░░░░░░░░░░░░   │
│  ░   [LOGO]    ░   │  8px minimum
│  ░░░░░░░░░░░░░░░   │
└────────────────────┘
```

### Do's ✅

- Use cyan primary logo on light and dark backgrounds.
- Scale proportionally (maintain aspect ratio).
- Maintain clear space.
- Use approved color variants (cyan, black, white).
- Use high-quality files (SVG for scalability, PNG for web).
- Keep centered or left-aligned.
- Use icon mark for small spaces.

### Don'ts ❌

- Don't distort or stretch the logo.
- Don't rotate at odd angles (only 0° or 90°).
- Don't add gradients, shadows, or glows.
- Don't change colors outside the approved palette.
- Don't place on low-contrast backgrounds.
- Don't crop, outline, or add borders.
- Don't combine with competing logos.
- Don't add effects like drop shadows.

---

## Resources

### Brand Assets

All brand assets are in the `logo/` directory:

- **SVG files** (scalable, recommended for web)
- **PNG files** (web-ready, transparent background)
- **PDF files** (print-ready, CMYK)

**Available Files:**

```text
logo/
├── arbordex-logo-cyan.svg
├── arbordex-logo-black.svg
├── arbordex-logo-white.svg
├── arbordex-mark.svg
├── arbordex-full-lockup.svg
└── [sizes available in PNG format]
```

### Questions or Issues?

1. Check this guide first.
2. Open an issue: <https://github.com/arbordex/brand/issues>
3. Tag with `#branding`

### License

Arbordex branding is licensed under **CC BY 4.0** (Creative Commons Attribution 4.0).

**You can:** Use, modify, share, and distribute.  
**You must:** Give credit to Arbordex and link to <https://github.com/arbordex>.

---

## Summary

Arbordex branding is **clear, warm, and professional**. Whether you're building a website, designing a print material, or writing copy - follow these guidelines to maintain consistency and reinforce our values:

- **Real** code and real impact
- **Clear** design and clear communication
- **Warm** approach to a growing community

🌳 Build DeFi. Grow Together. 💙
