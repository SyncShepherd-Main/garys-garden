# Gary Springer's Garden — Design Specification

> **This file is the source of truth for all design decisions on this site.**
> When making any update — adding pages, editing content, updating navigation — DO NOT change anything governed by this spec. If a requested change conflicts with this spec, flag it rather than silently overriding it.

---

## Typography

| Element | Specification |
|---|---|
| Font family | `'EB Garamond', Georgia, serif` — everywhere, no exceptions |
| Body text | 16px, line-height 1.85 |
| Navigation labels | 12px |
| Section labels | 11px, uppercase, letter-spacing 3–3.5px |
| Card type labels | 11px, uppercase, letter-spacing 2px |
| Footer | 13px |

**Never** introduce a second font. Never use system-ui, sans-serif, or any Google Font other than EB Garamond.

---

## Color Palette

### Backgrounds
| Token | Value | Used for |
|---|---|---|
| Page background | `#f5f3ed` | Warm parchment — all pages |
| Dark header/footer | `#2c2c2c` | Header, footer, dark callout blocks |
| Card background (stat) | `#ffffff` | Stat tiles, reference blocks |
| Light card background | `#f0ece4` | Further study blocks |

### Accent — Two schemes only

**Amber/gold** (newer pages — essays, saplings, biblical roots, immanuel moments):
| Token | Value |
|---|---|
| Primary accent | `#c77d00` |
| Hover accent | `#e8a020` |
| Border-bottom accent | `rgba(199,125,0,0.3)` |

**Forest green** (original framework viewers — 7-Tier, Recovery Model):
| Token | Value |
|---|---|
| Primary accent | `#4a7a3a` |
| Header background | `#1a2a1a` |

### Text
| Token | Value | Used for |
|---|---|---|
| Primary text | `#3a3a3a` | Body copy |
| Heading text | `#2c2c2c` | h1, h2, strong |
| Muted text | `#555` | em, secondary body |
| Label/meta text | `#888` | Card types, captions |
| Subdued text | `#999` | Header subtitles |

**Never** introduce new colors. Never use pure black (`#000`) or pure white (`#fff`) for text.

---

## Header

Every page header follows this exact structure:

```html
<header>
  <div class="inner">
    <div class="label">[Page type · Gary Springer's Garden]</div>
    <h1>[Page title]</h1>
    <p class="subtitle">[Page subtitle/tagline]</p>
    <div class="companion">[Back link + sibling page links]</div>
  </div>
</header>
```

- Background: `#2c2c2c`
- Bottom border: `3px solid #c77d00` (amber pages) or `3px solid #4a7a3a` (green pages)
- Padding: `32px 40px`
- Inner max-width: `800px` or `820px`
- h1: 30–32px, font-weight 400, color `#f5f3ed`
- Label: 11px, color `#c77d00`, uppercase, letter-spacing 3.5px
- Subtitle: 15px, color `#999`, italic
- Companion links: 13px, color `#c77d00`, border-bottom `rgba(199,125,0,0.3)`

**Never** change header colors. Never add icons, logos, or navigation elements to the page header.

---

## Top Navigation Bar (index.html only)

The index page has a fixed top nav with links to the main sections. This nav:
- Uses the existing color and font spec
- Must not be removed, restyled, or restructured
- Links must remain: 7-Tier Framework, Recovery Model, Biblical Roots, Immanuel Moments, Reading List (or equivalent)

When adding new top-level sections, add a link to this nav only if explicitly instructed.

---

## Page Layout

All content pages use a two-column sticky-nav layout:

```
[ nav sidebar 175px ] [ main content flex:1 ]
```

- Outer max-width: `800px` or `820px`, centered
- Gap: `44px`
- Padding: `40px 24px 80px`
- Nav: `position: sticky; top: 24px; align-self: flex-start`
- Nav rail: `border-left: 1px solid #d8d4cc; padding-left: 16px`

Mobile breakpoint (`≤680px`): stack vertically, nav goes full width and static.

---

## Navigation Sidebar (sticky nav)

Each section link uses a dot + label pattern:

```html
<button class="nav-btn" onclick="scrollTo('section-id')">
  <div class="nav-dot [active]" id="dot-section-id"></div>
  <span class="nav-label [active]" id="lbl-section-id">Section Title</span>
</button>
```

- Dot: 7px circle, inactive `#d0ccc4`, active `#c77d00` with glow `0 0 6px rgba(199,125,0,0.4)`
- Label: 12px, inactive `#888`, active `#2c2c2c` bold
- Dot tracks scroll position via JS — always include the scroll-tracking script

---

## Content Typography

```css
main h2 { font-size: 24–26px; font-weight: 400; color: #2c2c2c; 
          border-bottom: 1px solid #e0dcd4; padding-bottom: 8px; margin: 44–48px 0 8–10px; }
main h3 { font-size: 17px; font-weight: 600; color: #c77d00; margin: 28px 0 8px; }
main p  { font-size: 16px; line-height: 1.85; margin-bottom: 16px; }
main blockquote { border-left: 3px solid #c77d00; padding: 4px 0 4px 20px; margin: 24px 0; }
main blockquote p { font-size: 15.5px; font-style: italic; color: #555; }
main hr { border: none; border-top: 1px solid #e0dcd4; margin: 40–44px 0; }
```

---

## Footer

Every page footer:

```html
<footer>
  <p>A sapling in <a href="index.html">Gary Springer's Garden</a> — grounded in Scripture, informed by neuroscience, offered freely.</p>
</footer>
```

- Background: `#2c2c2c`
- Top border: `1px solid #3a3a3a`
- Padding: `24px 40px`
- Text align: center
- Text: 13px, color `#665544`
- Links: `#c77d00`

The footer tagline — *"grounded in Scripture, informed by neuroscience, offered freely"* — must appear on every page, unchanged.

**Never** modify the footer structure, colors, or tagline.

---

## Index Page Cards

Cards on the index page come in two styles:

**Green cards** (original framework viewers):
- Background: `#1a2a1a` or similar dark green
- Accent: `#4a7a3a`

**Amber cards** (essays, saplings, reference):
- Background: dark, amber-accented
- Card type label: `#c77d00`, 11px uppercase
- h2: ~18px, color `#f0ede6`
- Description: 14px, color `#ccc`
- Footer: format tag + arrow `→`

Do not change card colors, sizes, or hover behavior without explicit instruction.

---

## Sapling Draft Note

Working-draft pages include this block at the top of `<main>`:

```html
<div class="sapling-note">
  <p><strong>Working draft</strong> — [brief note]</p>
</div>
```

- Background: `#2c2c2c`
- Border-radius: `8px`
- Padding: `18px 24px`
- Text: 14.5px, color `#a09080`, italic
- `strong`: color `#c77d00`, non-italic

---

## What Never Changes

Regardless of what content is being added or edited:

1. **Font** — always EB Garamond
2. **Page background** — always `#f5f3ed`
3. **Header background** — always `#2c2c2c`
4. **Footer** — structure, tagline, colors unchanged
5. **Accent colors** — only `#c77d00` (amber) or `#4a7a3a` (green), never new colors
6. **Nav sidebar pattern** — dot + label, scroll-tracking JS, always present
7. **Max-width** — 800–820px content area
8. **Two-column layout** — nav sidebar + main content

---

## Adding New Pages

When adding a new sapling or essay page:

1. Copy the structure of an existing sapling page (e.g. `at-three-miles-per-hour.html`)
2. Use the amber color scheme unless explicitly told otherwise
3. Extract h2 headings for the sticky nav
4. Include scroll-tracking JS
5. Link back to `index.html` in the companion links
6. Use the standard footer tagline
7. Do not invent new CSS classes, colors, or layout patterns

---

## File Naming Convention

- All lowercase
- Words separated by hyphens
- Descriptive, not generic
- Examples: `roots-exposed-who-is-your-man.html`, `at-three-miles-per-hour.html`

---

*This spec was established March 2026. Update only with explicit instruction from Mark (site manager) on behalf of Gary Springer.*
