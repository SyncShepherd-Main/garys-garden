# Gary Springer's Garden

**Planting trees. Seeing what grows.**

A collection of frameworks for relationships, recovery, and the life of faith — grounded in Scripture, informed by neuroscience, and offered freely.

**Live site:** [https://syncshepherd-main.github.io/garys-garden/](https://syncshepherd-main.github.io/garys-garden/)

---

## What's Here

### Interactive Viewers

| Page | Description |
|------|-------------|
| [7-Tier Framework](https://syncshepherd-main.github.io/garys-garden/7-tier-framework.html) | A hierarchical model of relational and ideological ordering — from individual relationship with God at the root, outward through scriptural community, and into the realm of ideas, discernment, and darkness. Sidebar navigation with 7 expandable sections. |
| [Recovery Model](https://syncshepherd-main.github.io/garys-garden/holistic-recovery-model.html) | Eight integrated layers of recovery and restoration — mapping the FASTER Scale, brain science, voice of the heart, core needs, and practical boundaries against biblical anthropology. Sidebar navigation with 8 expandable sections. |
| [Biblical Roots](https://syncshepherd-main.github.io/garys-garden/biblical-roots-doc.html) | The scriptural architecture beneath the recovery model — including the full Gospel section: the Promise Plan, the Cup and the Cross, the Place of No Separation, and the Cry of the Adopted Child. |
| [Immanuel Moments](https://syncshepherd-main.github.io/garys-garden/immanuel-moments.html) | The personal story behind the frameworks. Moments where God planted something that didn't yet have a name — the three things, the praying hands, the orphan spirit, the place of hearing. |

### Saplings

Working drafts — little trees that might grow to be a big forest.

| Page | Type | Description |
|------|------|-------------|
| [ACEs: The Wound Beneath the Wound](https://syncshepherd-main.github.io/garys-garden/aces-layer-proposal.html) | Sapling | Adverse Childhood Experiences as the missing ground floor of the recovery model — launching from *Paper Tigers* and the CDC-Kaiser ACE Study. Proposed new layer. |
| [At Three Miles Per Hour](https://syncshepherd-main.github.io/garys-garden/at-three-miles-per-hour.html) | Sapling | Walking-speed theology — a meditation on presence, pace, and what becomes visible when you slow down. 10 sections with sidebar navigation. |
| [The Songs I Chose for Them](https://syncshepherd-main.github.io/garys-garden/the-songs-i-chose-for-them.html) | Sapling | The soundtrack of fatherhood — songs chosen for children and what they carry. 7 sections with sidebar navigation. |
| [Roots Exposed: Who Is Your Man?](https://syncshepherd-main.github.io/garys-garden/roots-exposed-who-is-your-man.html) | Sapling | Identity and the question beneath the question. 6 sections with sidebar navigation. |
| [The Gardener Does Not Uproot](https://syncshepherd-main.github.io/garys-garden/the-gardener-does-not-uproot.html) | Sapling | Patience, pruning, and how God tends what He planted. 8 sections with sidebar navigation. |
| [The Best Wine Saved for Last](https://syncshepherd-main.github.io/garys-garden/the-best-wine-saved-for-last.html) | Sapling | What the miracle at Cana reveals about God's timing and generosity. 6 sections with sidebar navigation. |
| [Relaxing in the Run](https://syncshepherd-main.github.io/garys-garden/relaxing-in-the-run.html) | Personal Statement | Gary's personal statement — not a working draft. 5 sections with sidebar navigation. |
| [Clarity AI: Making Something Possible](https://syncshepherd-main.github.io/garys-garden/clarity-ai-making-something-possible.html) | Record | A record of how AI tools helped bring the garden into being. 8 sections with sidebar navigation. |

### Reference & Study

| Page | Description |
|------|-------------|
| [Recommended Reading](https://syncshepherd-main.github.io/garys-garden/recommended-reading.html) | A complete bibliography for the Eight-Layer Recovery Model, the 7-Tier Framework, and the Gospel foundation — including a curated 10-step reading pathway and a "Pace, Presence & the Parish" section. Interactive sidebar with 30+ books. |
| [Paul & the Old Testament](https://syncshepherd-main.github.io/garys-garden/paul-essay.html) | How Paul's letters reshaped the tradition he loved — and what Andy Crouch's framework of cultural artifacts reveals about why young believers major in Paul over Jesus. |

### Visual Reference

| Page | Description |
|------|-------------|
| [7-Tier Flowchart](https://syncshepherd-main.github.io/garys-garden/7-tier-flowchart-view.html) | A visual overview of all seven tiers with scripture references and the Jeremiah 17 Diagnostic. |

### Source Documents

These pages render the raw markdown source files with full formatting, navigation, and scroll-to-top.

| Page | Source File | Description |
|------|-------------|-------------|
| [7-Tier Full Text](https://syncshepherd-main.github.io/garys-garden/7-tier-full-text.html) | `7-Tier-Framework.md` | Complete source: epistemological statement, all seven tiers, biblical tap roots, key concepts, and cross-reference structure. |
| [Eight-Layer Reference](https://syncshepherd-main.github.io/garys-garden/eight-layer-reference.html) | `seven-layers.md` | Full written reference: core equation, each layer's framework, diagnostic workflow, VIM architecture, and cross-reference matrix. |
| [Biblical Roots Source](https://syncshepherd-main.github.io/garys-garden/biblical-roots-source.html) | `biblical-roots.md` | The full biblical roots document with the newly added Gospel section. |
| [Immanuel Moments Source](https://syncshepherd-main.github.io/garys-garden/immanuel-moments-source.html) | `immanuel-moments.md` | Plain-text source for the Immanuel Moments testimony page. |

---

## Site-Wide Features

- **Two-row navigation bar** — Site name centered on row 1, page links on row 2. "Saplings" dropdown menu links to all 8 essay pages. Hamburger menu on mobile.
- **Scroll-to-top button** — Floating 56px circle (bottom-right) on all 20 pages. Appears after scrolling 400px.
- **Sticky sidebar navigation** — Dot + label pattern with scroll-tracking JS on all sapling and interactive viewer pages. Uses `scrollToSection()` function.
- **Consistent footer** — "Planted by Gary Springer — grounded in Scripture, informed by neuroscience, offered freely." on every page.

---

## Technical Details

- **Hosting:** GitHub Pages via GitHub Actions (auto-deploys on push to `main`)
- **Stack:** Pure static HTML/CSS/JS — no build tools, no frameworks, no dependencies
- **Pages:** 20 HTML pages, 9 markdown source files, 2 images
- **Max content width:** 1200px (all pages)
- **Font:** EB Garamond (Google Fonts), fallback: Georgia, serif
- **Body text:** 18px, line-height 1.85
- **Nav link font:** 18px (two-row centered layout)
- **Markdown rendering:** Custom client-side `parseMarkdown()` in each source document page (fetches `.md` files and renders to HTML)
- **Responsive:** Hamburger menu on mobile (< 700px breakpoint), fluid card grid on homepage, sidebar collapses on mobile (< 680px)

### Color Scheme (Blue)

| Token | Value | Used For |
|-------|-------|----------|
| Page background | `#f5f3ed` | Warm parchment — all pages |
| Deep navy | `#1a2040` | Header/footer backgrounds, headings, strong text |
| Steel blue | `#4a78b4` | Accent color — links, labels, borders, active dots |
| Sky blue | `#8ab0cc` | Light text on dark backgrounds, home link, footer text |
| Nav bar bg | `#1a1a1a` | Top navigation bar background |
| Body text | `#2e4060` | Primary body copy |
| Muted text | `#666` | Blockquotes, italics, secondary text |
| Sapling note text | `#c8b8a8` | Working draft note text on dark background |

### Key CSS Patterns

- **Sidebar nav dot active:** `background: #4a78b4; box-shadow: 0 0 6px rgba(74,120,180,0.4);`
- **Scroll function:** `scrollToSection(id)` — renamed from `scrollTo` to avoid conflict with native `window.scrollTo`
- **Scroll-to-top trigger:** Shows after `window.scrollY > 400`
- **Dropdown close:** Click-outside listener removes `.open` class from `.nav-dropdown`

---

## File Structure

```
garys-garden/
  index.html                                Homepage — card grid linking to all pages
  7-tier-framework.html                     Interactive 7-tier viewer (sidebar nav, JS renderers)
  holistic-recovery-model.html              Interactive 8-layer recovery viewer (sidebar nav, JS renderers)
  biblical-roots-doc.html                   Biblical roots interactive viewer (hardcoded content)
  immanuel-moments.html                     Immanuel Moments testimony (hardcoded content)
  recommended-reading.html                  Recommended reading interactive viewer (sidebar nav)
  paul-essay.html                           Paul essay viewer (renders paul-and-the-old-testament.md)
  aces-layer-proposal.html                  Sapling — ACEs layer proposal
  at-three-miles-per-hour.html              Sapling — walking-speed theology
  the-songs-i-chose-for-them.html           Sapling — the soundtrack of fatherhood
  roots-exposed-who-is-your-man.html        Sapling — identity and the deeper question
  the-gardener-does-not-uproot.html         Sapling — patience and pruning
  the-best-wine-saved-for-last.html         Sapling — the miracle at Cana
  relaxing-in-the-run.html                  Personal statement (not a draft)
  clarity-ai-making-something-possible.html Record — how AI helped build the garden
  7-tier-full-text.html                     Source viewer (renders 7-Tier-Framework.md)
  eight-layer-reference.html                Source viewer (renders seven-layers.md)
  biblical-roots-source.html                Source viewer (renders biblical-roots.md)
  immanuel-moments-source.html              Source viewer (renders immanuel-moments.md)
  7-tier-flowchart-view.html                Flowchart image viewer with navigation
  7-tier-flowchart.png                      Visual flowchart of the 7-tier framework
  Saplings.jpg                              Saplings section hero image
  7-Tier-Framework.md                       Source: 7-tier relational framework
  seven-layers.md                           Source: 8-layer recovery model
  biblical-roots.md                         Source: biblical roots theological supplement
  immanuel-moments.md                       Source: Immanuel Moments testimony
  paul-and-the-old-testament.md             Source: Paul & the Old Testament essay
  recommended-reading.md                    Source: bibliography and reading list
  aces-layer-proposal.md                    Source: ACEs layer proposal essay
  at-three-miles-per-hour.md                Source: At Three Miles Per Hour essay
  the-songs-i-chose-for-them.md             Source: The Songs I Chose for Them essay
  roots-exposed-who-is-your-man.md          Source: Roots Exposed essay
  the-gardener-does-not-uproot.md           Source: The Gardener Does Not Uproot essay
  the-best-wine-saved-for-last.md           Source: The Best Wine Saved for Last essay
  relaxing-in-the-run.md                    Source: Relaxing in the Run statement
  clarity-ai-making-something-possible.md   Source: Clarity AI record
  DESIGN_SPEC.md                            Design specification (source of truth for styles)
  SITE-DOCUMENTATION.md                     Site documentation
  .github/workflows/static.yml              GitHub Pages deployment workflow
```

## Update History

| Date | Changes |
|------|---------|
| Mar 10, 2026 | Added 7 new sapling pages from Gary's updates. Updated recommended reading with "Pace, Presence & the Parish" section. Converted entire site to blue color scheme. Added site-wide nav bar with Saplings dropdown. Fixed sidebar scroll (renamed `scrollTo` → `scrollToSection`). Widened all pages to 1200px. Bumped body font to 18px. Lightened muted text colors. Added 56px scroll-to-top button to all pages. |
| Mar 8, 2026 | Added ACEs layer proposal as first sapling. Applied Orphan Spirit privacy rewrite. |
| Feb 2026 | Converted color scheme from green/amber to blue. Expanded Immanuel Moments. Added Earley to Reading List. |

---

## License

This work is offered freely. No rights reserved.
