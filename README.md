# Arbor DEX Brand System

Welcome to the **Arbor DEX Brand System**. This repository contains all visual and verbal branding assets for Arbor DEX, maintaining consistency across communications, products, and materials.

**Related Repositories:**

- **[Arbor DEX (DEX repo)](https://github.com/arbordex/dex)** – The main DEX application product
- **[Arbor DEX Brand (Brand repo)](https://github.com/arbordex/brand)** – Branding assets, colors, and typography (you are here)

---

## 🎯 Get Started

### **[BRAND.md](./BRAND.md)** ← START HERE

A **single, consolidated** source for all brand guidelines:

- Brand essence, vision, and values
- Visual identity (logo, colors, typography)
- Voice & tone
- Complete usage guidelines
- Logo specifications
- Quick CSS variables and references

---

## 🎨 Quick Reference

### Colors

```text
Primary Cyan:      #00FFFF (logo, CTA, accents)
Dark Teal:         #004B57 (dark backgrounds)
Ink Black:         #05070A (light mode text)
Clean White:       #FFFFFF (dark mode text)
Light Teal:        #55F2E3 (hover, secondary)
Light Gray:        #F8F9FA (light backgrounds)
Soft Gray:         #E8E8E8 (dividers)
Medium Slate:      #1A1F3A (secondary text)
```

See **[BRAND.md](./BRAND.md#colors)** for full palette and usage.

### Typography

**Fonts:**

- **Inter** – UI, web, marketing (weights: 400, 500, 600, 700)
- **IBM Plex Mono** – Code, technical content

**Import:**

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=IBM+Plex+Mono:wght@400;600&display=swap" rel="stylesheet">
```

See **[BRAND.md](./BRAND.md#typography)** for type scale and CSS setup.

### Logo

| Primary | Mono | Mark (favicon default) | Wordmark |
| --- | --- | --- | --- |
| ![Primary cyan logo](./logo/arbordex-logo-cyan.svg) | ![Mono logo](./logo/arbordex-logo-bw.svg) | ![Cyan mark](./logo/arbordex-mark-cyan.svg) | ![Cyan wordmark](./logo/arbordex-wordmark-cyan.svg) |

- Files in `logo/`: `arbordex.svg` (legacy name of the primary), `arbordex-logo-cyan.svg`, `arbordex-logo-bw.svg`, `arbordex-mark-cyan.svg`, `arbordex-mark-bw.svg`, `arbordex-wordmark-cyan.svg`, `arbordex-wordmark-bw.svg`.
- **Mark:** Use for favicons (default), app icons, avatars, and tight UI spaces. Avoid recoloring or placing in containers.
- **Wordmark:** Use where text clarity matters (nav bars, slim headers); avoid at tiny sizes or on low-contrast photos.
- **Logo:** Use cyan for most cases; switch to bw only for single-ink or emboss scenarios. Maintain clear space ≥ 8px.

See **[BRAND.md](./BRAND.md#logo-usage)** for detailed sizing and usage guidelines.

---

## 📋 Document Guide

| Document | Contains | Read Time |
|----------|----------|-----------|
| **BRAND.md** | Everything (consolidated) | 15 min |
| **README.md** | This quick start | 3 min |
| **logo/README.md** | Logo file details | 2 min |

---

## ✨ Voice & Tone

**Arbordex sounds:**

- Warm and approachable
- Honest and transparent
- Clear and direct
- Professional and competent

**Examples:**

- ✅ "Build, explore, and understand DeFi from the ground up."
- ✅ "Code is meant to be read and modified."
- ❌ "Enterprise-grade blockchain infrastructure." (Too corporate)
- ❌ "Cutting-edge AI-powered DeFi solutions." (Hype)

See **[BRAND.md](./BRAND.md#voice--tone)** for detailed guidelines.

---

## 🚀 Using the Brand

### In a Website

1. Logo: Use `arbordex-logo-cyan.svg` in header (48–64px); switch to `arbordex-logo-bw.svg` only for single-ink.
2. Mark: Use `arbordex-mark-cyan.svg` for the favicon (default) and pinned tabs.
3. Colors: Primary cyan `#00FFFF`, text `#05070A` (light) or `#FFFFFF` (dark)
4. Fonts: Inter for everything, IBM Plex Mono for code
5. Contrast: Ensure text is readable (4.5:1 minimum)

### In Documentation

1. Logo: `arbordex-mark-cyan.svg` (24–48px) next to headings; pair with `arbordex-wordmark-cyan.svg` if you need readable text.
2. Code blocks: Use monospace font (IBM Plex Mono)
3. Tone: Clear, conversational, no jargon

### In Social Media

1. Avatar: `arbordex-mark-cyan.svg` (128–512px); avoid recoloring.
2. Banner: Full logo with cyan background; keep clear space.
3. Posts: Use voice examples from BRAND.md

### In Print

1. Logo: `arbordex-logo-bw.svg` (0.75"+ size) for single-ink; cyan on white when color printing is available.
2. Colors: Use black and white only, or cyan on white
3. Fonts: Make sure Inter is available or use serif fallback

---

## Logo Do/Don’t (visual)

| Do | Don’t |
| --- | --- |
| <img src="./logo/arbordex-logo-cyan.svg" alt="Logo on light" width="180" style="background:#ffffff;padding:12px;border:1px solid #e8e8e8;"> | <img src="./logo/arbordex-logo-cyan.svg" alt="Recolored (don’t)" width="180" style="filter:hue-rotate(120deg) brightness(0.8);padding:12px;border:1px solid #e8e8e8;"> |
| Use approved cyan on clean, high-contrast backgrounds. | Don’t recolor outside the palette. |
| <img src="./logo/arbordex-mark-cyan.svg" alt="Mark on dark" width="72" style="background:#0b0f1a;padding:10px;border-radius:12px;"> | <img src="./logo/arbordex-mark-cyan.svg" alt="Outlined (don’t)" width="72" style="background:#ffffff;padding:10px;border:2px dashed #ff4d4f;"> |
| Use the mark alone for favicons, avatars, and small UI. | Don’t add outlines, containers, or effects. |

---

## 📝 Commit Convention

We follow **scoped conventional commits** with a semantic structure that makes commit history scannable and automated tooling-friendly.

### Format

```text
<type>(<scope>): <short description>

<long description>

<footer>
```

### Type & Scope

| Type | Use | Scope Examples |
|------|-----|----------------|
| **feat** | New feature or asset | `logo`, `colors`, `typography`, `brand-guide` |
| **fix** | Bug or correction | `logo`, `svg`, `colors`, `spacing` |
| **docs** | Documentation update | `readme`, `brand-guide`, `usage` |
| **style** | Style/formatting (no logic) | `colors`, `fonts` |
| **refactor** | Code restructure | `brand-guide`, `asset-system` |
| **perf** | Performance improvement | `svg-optimization`, `asset-size` |
| **chore** | Maintenance/tooling | `deps`, `ci`, `config` |
| **ci** | CI/CD changes | `github-actions`, `workflow` |

### Examples

```bash
feat(logo): add wordmark variants in cyan and monochrome

Add arbordex-wordmark-cyan.svg and arbordex-wordmark-bw.svg
for horizontal-space-constrained layouts.

Fixes #42
Closes #45
```

```bash
fix(svg): adjust mark viewBox to prevent bottom cropping

Increased viewBox height from 390 to 431 to ensure full
canopy is visible in arbordex-mark-bw.svg and
arbordex-mark-cyan.svg.

Related: #38
```

```bash
docs(readme): update logo section with new asset files

Replace outdated file list with regenerated SVG assets.
Add usage guidance for mark (favicons), wordmark (tight
spaces), and full logo.

Closes #50
```

### Footer Format

Include references to GitHub issues/PRs in the footer:

- `Fixes #<number>`  -  Closes the issue
- `Closes #<number>`  -  Closes the issue
- `Related: #<number>`  -  References without closing
- `Refs: <url>`  -  External references

### Writing Tips

1. **Type**: Use lowercase; match the semantic meaning of your change.
2. **Scope**: Use lowercase, match actual areas of the repo (logo, colors, docs, etc.).
3. **Short description**: Imperative mood ("add", "fix", "update"), max 50 chars, no period.
4. **Long description**: Wrap at 72 chars, explain *why* and *what*, not *how*; use bullets for clarity.
5. **Footer**: Always link to issues/PRs so reviewers have context.

---

## ✅ Before Publishing

- [ ] Logo is one of the approved variants (cyan/black/white full logo or cyan mark)
- [ ] Logo has 8px clear space
- [ ] Colors match the palette
- [ ] Text uses Inter or IBM Plex Mono
- [ ] Text contrast is ≥ 4.5:1 (WCAG AA)
- [ ] Messaging is warm and honest
- [ ] Design works on light and dark backgrounds

---

## ❓ FAQ

**Q: Which logo should I use?**
A: Cyan for most uses. Use black for print. Use white for dark backgrounds. Use icon mark for small spaces.

**Q: Can I change the logo colors?**
A: No, use approved variants only (cyan, black, white monochrome). See BRAND.md for details.

**Q: What font stack should I use?**
A: Inter for UI. Copy from BRAND.md → Typography → CSS Stack section.

**Q: How small can the logo be?**
A: 24px minimum for digital, 0.75" for print. At very small sizes, use the icon mark.

**Q: Can I add shadows or effects?**
A: No. Keep the logo flat and clean.

**Q: Who do I contact with brand questions?**
A: Open an issue at <https://github.com/arbordex/brand/issues> and tag with `#branding`.

---

## 📄 License

Arbordex branding is licensed under **CC BY 4.0** (Creative Commons Attribution 4.0).

**You can:** Use, modify, share, commercialize.  
**You must:** Credit Arbordex and link to <https://github.com/arbordex>.

---

🌳 **Build DeFi. Grow Together.** 💙

---

**Last Updated:** December 2025
**Maintained by:** Arbordex Brand Team
