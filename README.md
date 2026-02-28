# ETCswap Brand Guidelines

Official brand assets and guidelines for ETCswap — the leading decentralized exchange on Ethereum Classic.

**Last Updated:** February 2026

---

## Brand Overview

**ETCswap** is a suite of decentralized exchange products on Ethereum Classic. Our visual identity reflects the technical precision and trustless nature of DeFi while maintaining approachability through a distinctive neon green accent against dark interfaces.

**Tagline:** Decentralized Exchange on Ethereum Classic

**Products:**
- **ETCswap V2** — Core AMM DEX (`v2.etcswap.org`)
- **ETCswap V3** — Concentrated liquidity DEX (`v3.etcswap.org`)
- **ETCswap Launchpad** — Token creation and bonding curves
- **ETCswap Analytics** — On-chain DEX analytics

**Community:**
- GitHub: [github.com/etcswap](https://github.com/etcswap)
- X: [@ETCswap_org](https://x.com/ETCswap_org)
- Telegram: [@ETCswap_org](https://t.me/ETCswap_org)

---

## Logo System

### Logomark

The ETCswap logomark is a geometric 3-path mark representing the flow of decentralized exchange — assets moving through interconnected paths.

| Variant | File | Usage |
|---------|------|-------|
| **Green** (Primary) | [`logo/logomark-green.svg`](logo/logomark-green.svg) | Default. Use on dark and light backgrounds. |
| **White** | [`logo/logomark-white.svg`](logo/logomark-white.svg) | On solid dark backgrounds where green lacks contrast. |
| **Black** | [`logo/logomark-black.svg`](logo/logomark-black.svg) | On solid light backgrounds, print, monochrome contexts. |

**PNG exports** are available in [`logo/png/`](logo/png/) at 512, 256, 128, and 64px.

### Wordmark

The ETCswap wordmark uses **DM Sans Bold** with tight tracking (-0.02em).

| Variant | File | Usage |
|---------|------|-------|
| **White** | [`logo/wordmark-white.svg`](logo/wordmark-white.svg) | On dark backgrounds. |
| **Black** | [`logo/wordmark-black.svg`](logo/wordmark-black.svg) | On light backgrounds. |

### Lockup (Logo + Text)

Horizontal lockup with logomark left, wordmark right. The logomark is always green; text color adapts to background.

| Variant | File | Usage |
|---------|------|-------|
| **White text** | [`logo/lockup-horizontal-white.svg`](logo/lockup-horizontal-white.svg) | Dark backgrounds. |
| **Black text** | [`logo/lockup-horizontal-black.svg`](logo/lockup-horizontal-black.svg) | Light backgrounds. |

### Usage Rules

**Clear Space:** Maintain a minimum clear space equal to the height of the logomark on all sides.

**Minimum Sizes:**
- Digital: 32px height
- Print: 10mm height

**Do:**
- Use provided SVG files for maximum quality
- Maintain aspect ratio
- Use approved color variants only

**Don't:**
- Stretch, skew, or rotate the logo
- Add shadows, outlines, or effects
- Recolor outside the approved palette
- Place on visually busy backgrounds without sufficient contrast
- Modify the geometry or proportions

---

## Color Palette

ETCswap uses a dark-first design language with a distinctive neon green accent.

### Primary

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| **ETCswap Green** | `#33FF99` | `51, 255, 153` | Primary accent, CTAs, logo, interactive elements |
| **Green Hover** | `#00F77C` | `0, 247, 124` | Hover states |
| **Green Active** | `#00BC5E` | `0, 188, 94` | Active/pressed states |
| **Green Subtle** | `rgba(51, 255, 153, 0.08)` | — | Tinted backgrounds, badge fills |
| **Green Glow** | `rgba(51, 255, 153, 0.4)` | — | Text selection, glow effects |

### Dark Mode (Default)

| Color | Hex | Usage |
|-------|-----|-------|
| **Background** | `#131313` | Primary surface (V2, V3) |
| **Deep Background** | `#030508` | Landing page, deep dark surfaces |
| **Surface** | `#2C2F36` | Cards, elevated containers |
| **Elevated** | `#40444F` | Inputs, secondary surfaces |

### Light Mode

| Color | Hex | Usage |
|-------|-----|-------|
| **Background** | `#FFFFFF` | Primary surface |
| **Deep Background** | `#F7F8FA` | Subtle surface separation |
| **Surface** | `#EDEEF2` | Cards, containers |
| **Elevated** | `#CED0D9` | Inputs, secondary surfaces |

### Text Colors

| Role | Dark Mode | Light Mode |
|------|-----------|------------|
| **Primary** | `#FFFFFF` | `#131313` |
| **Secondary** | `#C3C5CB` | `#565A69` |
| **Muted** | `#6C7284` | `#888D9B` |
| **Subtle** | `#565A69` | `#C3C5CB` |

### Semantic Colors

| Meaning | Hex | Usage |
|---------|-----|-------|
| **Success** | `#33FF99` | Positive actions, confirmations |
| **Error** | `#FD025D` | Errors, destructive actions |
| **Warning** | `#F3841E` | Cautions, pending states |
| **Info** | `#33FFF4` | Informational highlights |

### Color Distribution

Follow the **60-30-10 rule:**
- **60%** — Background surfaces (`#131313` dark / `#FFFFFF` light)
- **30%** — Text and secondary elements
- **10%** — Brand green accent (`#33FF99`) — CTAs, active states, highlights

### Accessibility

All text/background combinations meet **WCAG AA** contrast standards:
- `#FFFFFF` on `#131313` — 18.3:1 (AAA)
- `#33FF99` on `#131313` — 12.6:1 (AAA)
- `#131313` on `#33FF99` — 12.6:1 (AAA)
- `#C3C5CB` on `#131313` — 9.8:1 (AAA)

### Design Tokens

Pre-built token files for integration:
- **CSS Custom Properties:** [`tokens/colors.css`](tokens/colors.css)
- **JSON (machine-readable):** [`tokens/colors.json`](tokens/colors.json)
- **Tailwind CSS 4:** [`tokens/tailwind.css`](tokens/tailwind.css)

---

## Typography

### Primary Font: DM Sans

[DM Sans](https://fonts.google.com/specimen/DM+Sans) is a geometric sans-serif from Google Fonts. It provides clean legibility at small sizes and distinctive character at large display sizes.

**Weights:**
| Weight | Value | Usage |
|--------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Labels, navigation |
| Semibold | 600 | Subheadings, card titles |
| Bold | 700 | Headings, hero text, wordmark |

**Letter Spacing:** `-0.018em` for body, `-0.02em` for headings

**Fallback Stack:**
```css
font-family: 'DM Sans', system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
```

### Google Fonts Import

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,400;0,500;0,600;0,700;1,400&display=swap" rel="stylesheet">
```

### Next.js Import

```typescript
import { DM_Sans } from 'next/font/google';

const dmSans = DM_Sans({
  variable: '--font-dm-sans',
  subsets: ['latin'],
});
```

### Type Scale

| Level | Size | Weight | Usage |
|-------|------|--------|-------|
| Display | `text-5xl` (3rem) | Bold (700) | Hero headlines |
| H1 | `text-4xl` (2.25rem) | Bold (700) | Page titles |
| H2 | `text-2xl` (1.5rem) | Bold (700) | Section headings |
| H3 | `text-lg` (1.125rem) | Semibold (600) | Card titles |
| Body | `text-base` (1rem) | Regular (400) | Body text |
| Small | `text-sm` (0.875rem) | Regular (400) | Secondary text |
| Caption | `text-xs` (0.75rem) | Medium (500) | Labels, badges |

---

## Design Language

### Dark-First Philosophy

ETCswap interfaces default to dark mode. Dark backgrounds reduce eye strain during extended trading sessions and create natural contrast for the green accent color.

- Use `#131313` as the standard dark background (V2, V3 products)
- Use `#030508` for landing pages and marketing surfaces (deeper, richer dark)
- Light mode is supported but dark mode is the primary design target

### Glass Card Pattern

For elevated containers, use the glassmorphism effect:

```css
.glass {
  background: rgba(10, 13, 18, 0.6);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.08);
}
```

### Green Glow Effects

Use sparingly for emphasis and brand presence:

```css
/* Text glow (hero headlines only) */
text-shadow:
  0 0 20px rgba(51, 255, 153, 0.15),
  0 0 40px rgba(51, 255, 153, 0.08),
  0 0 80px rgba(51, 255, 153, 0.04);

/* Button hover glow */
box-shadow: 0 0 20px rgba(51, 255, 153, 0.3);
```

### Button Styles

```css
/* Primary CTA */
background: #33FF99;
color: #131313;
border-radius: 12px;
font-weight: 600;
transition: background 150ms ease-in;

/* Primary CTA Hover */
background: #00F77C;
```

### Spacing Rhythm

Use an 8px base grid:

| Token | Value | Usage |
|-------|-------|-------|
| `sm` | 8px | Tight internal spacing |
| `md` | 12px | Default component padding |
| `lg` | 24px | Section gaps, card padding |
| `xl` | 48px | Between major sections |
| `2xl` | 80px | Hero/section vertical padding |

---

## Product Branding

All ETCswap products share the **same logomark, color palette, typography, and design language.** Products are differentiated only by name and URL.

### Product Naming Convention

- Always use "ETCswap" as one word, with exact capitalization: **ETC** (uppercase) + **swap** (lowercase)
- Product names follow the brand: "ETCswap V2", "ETCswap V3", "ETCswap Launchpad", "ETCswap Analytics"
- In technical contexts: `@etcswap/v2-interface`, `@etcswap/v3-interface`

### Product Domains

| Product | Domain |
|---------|--------|
| Landing / Main | `etcswap.org` |
| V2 DEX | `v2.etcswap.org` |
| V3 DEX | `v3.etcswap.org` |
| Launchpad | TBD |
| Analytics | TBD |

### Product OG Images

Pre-built social cards for each product are in [`social/`](social/):
- [`og-etcswap.png`](social/og-etcswap.png) — Main brand (1200x630)
- [`og-v2.png`](social/og-v2.png) — V2 DEX
- [`og-v3.png`](social/og-v3.png) — V3 DEX
- [`og-launchpad.png`](social/og-launchpad.png) — Launchpad
- [`og-analytics.png`](social/og-analytics.png) — Analytics

SVG source files are also provided for customization.

---

## Favicon Implementation

### Files

All favicon assets are in [`favicon/`](favicon/):

| File | Size | Format |
|------|------|--------|
| `favicon.svg` | Any | SVG (preferred) |
| `favicon.ico` | 16+32+48 | ICO (legacy) |
| `favicon-16x16.png` | 16x16 | PNG |
| `favicon-32x32.png` | 32x32 | PNG |
| `favicon-48x48.png` | 48x48 | PNG |
| `apple-touch-icon.png` | 180x180 | PNG |
| `android-chrome-192x192.png` | 192x192 | PNG |
| `android-chrome-512x512.png` | 512x512 | PNG |

### HTML Snippet

```html
<link rel="icon" type="image/svg+xml" href="/favicon.svg">
<link rel="icon" type="image/x-icon" href="/favicon.ico">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#33FF99">
```

### Web Manifest Template

See [`favicon/site.webmanifest`](favicon/site.webmanifest) — copy and customize `name` and `short_name` per product.

---

## Social Media

### Open Graph Setup

```html
<meta property="og:title" content="ETCswap — Decentralized Exchange on Ethereum Classic">
<meta property="og:description" content="Swap tokens, provide liquidity, and trade on Ethereum Classic.">
<meta property="og:image" content="https://etcswap.org/og-image.png">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:image:type" content="image/png">
<meta property="og:type" content="website">
<meta property="og:url" content="https://etcswap.org">
```

### Twitter Card

```html
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="ETCswap — Decentralized Exchange on Ethereum Classic">
<meta name="twitter:description" content="Swap tokens, provide liquidity, and trade on Ethereum Classic.">
<meta name="twitter:image" content="https://etcswap.org/og-image.png">
```

### Profile Picture

Use `logomark-green.svg` or `logomark-green-512.png` for profile pictures across social platforms.

---

## Repository Structure

```
brand/
├── README.md                          # This file
├── logo/
│   ├── logomark-green.svg             # Primary mark (#33FF99)
│   ├── logomark-white.svg             # White variant
│   ├── logomark-black.svg             # Black variant
│   ├── wordmark-white.svg             # "ETCswap" text (white)
│   ├── wordmark-black.svg             # "ETCswap" text (black)
│   ├── lockup-horizontal-white.svg    # Logo + text (white)
│   ├── lockup-horizontal-black.svg    # Logo + text (black)
│   └── png/                           # Pre-rendered PNGs
│       ├── logomark-green-512.png
│       ├── logomark-green-256.png
│       ├── logomark-green-128.png
│       ├── logomark-green-64.png
│       ├── logomark-white-512.png
│       ├── logomark-white-256.png
│       └── logomark-black-512.png
├── favicon/
│   ├── favicon.svg                    # SVG favicon
│   ├── favicon.ico                    # ICO (multi-size)
│   ├── favicon-16x16.png
│   ├── favicon-32x32.png
│   ├── favicon-48x48.png
│   ├── apple-touch-icon.png           # 180x180
│   ├── android-chrome-192x192.png
│   ├── android-chrome-512x512.png
│   └── site.webmanifest               # Web app manifest template
├── social/
│   ├── og-etcswap.svg / .png          # Main brand (1200x630)
│   ├── og-v2.svg / .png               # V2 product
│   ├── og-v3.svg / .png               # V3 product
│   ├── og-launchpad.svg / .png        # Launchpad
│   └── og-analytics.svg / .png        # Analytics
└── tokens/
    ├── colors.css                     # CSS custom properties
    ├── colors.json                    # Machine-readable palette
    └── tailwind.css                   # Tailwind CSS 4 theme
```

---

## Quick Reference

| Element | Value |
|---------|-------|
| Primary Color | `#33FF99` |
| Dark Background | `#131313` |
| Deep Background | `#030508` |
| Light Background | `#FFFFFF` |
| Font | DM Sans |
| Font Weights | 400, 500, 600, 700 |
| Border Radius (buttons) | 12px |
| Border Radius (cards) | 16px |
| Theme Color (meta) | `#33FF99` |
| OG Image Size | 1200 x 630 |

---

## License

ETCswap brand assets are provided for use in connection with ETCswap products and the Ethereum Classic ecosystem. Contact the ETCswap team for usage outside these contexts.
