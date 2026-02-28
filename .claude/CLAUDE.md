# ETCswap Brand Repository

## Project Context

This is the canonical brand asset repository for ETCswap — a suite of decentralized exchange products on Ethereum Classic. It contains logos, favicons, social cards, design tokens, and comprehensive brand guidelines.

**Repo:** `etcswap/brand` (GitHub)
**Type:** Brand assets (no build system, no dependencies)

## Structure

- `logo/` — Logomark (green/white/black), wordmark, lockup SVGs + PNGs
- `favicon/` — Complete favicon package (SVG, ICO, PNGs, manifest)
- `social/` — OG images for all products (SVG sources + rendered PNGs)
- `tokens/` — Design tokens (CSS, JSON, Tailwind CSS 4)
- `README.md` — Comprehensive brand guidelines

## Brand Identity

- **Primary color:** `#33FF99` (neon green)
- **Dark background:** `#131313` (standard) / `#030508` (deep)
- **Font:** DM Sans (Google Fonts)
- **Design philosophy:** Dark-first, glass effects, neon green accents

## Key Rules

1. The logomark SVG (`logo/logomark-green.svg`) is the canonical logo — 1,092 bytes, 3 vector paths
2. All products share the same logomark, colors, and typography
3. Product differentiation is by name only (V2, V3, Launchpad, Analytics)
4. PNGs are generated from SVGs using ImageMagick (`convert`)
5. OG images follow the same dark gradient + green grid template

## Commands

```bash
# Generate PNGs from SVG (requires ImageMagick)
convert -background none logo/logomark-green.svg -resize 512x512 logo/png/logomark-green-512.png

# Generate favicon ICO
convert favicon/favicon-16x16.png favicon/favicon-32x32.png favicon/favicon-48x48.png favicon/favicon.ico
```

## Boundaries

### Always Do
- Use SVG as the source of truth for all logos
- Maintain the exact `#33FF99` brand green
- Keep the logomark geometry unchanged

### Ask First
- Adding new product brand packages
- Changing the color palette
- Modifying the logo geometry

### Never Do
- Commit .env files or secrets
- Modify the logomark paths (they are the brand mark)
- Use colors outside the defined palette
