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

### Source Documents

| Page | Source File | Description |
|------|-------------|-------------|
| [7-Tier Full Text](https://syncshepherd-main.github.io/garys-garden/7-tier-full-text.html) | `7-Tier-Framework.md` | Complete source document: epistemological statement, all seven tiers with biblical tap roots, key concepts, and cross-reference structure. |
| [Eight-Layer Reference](https://syncshepherd-main.github.io/garys-garden/eight-layer-reference.html) | `seven-layers.md` | Full written reference: core equation, each layer's framework, diagnostic workflow, VIM architecture, and cross-reference matrix. |
| [Biblical Roots](https://syncshepherd-main.github.io/garys-garden/biblical-roots-doc.html) | `biblical-roots.md` | Theological supplement tracing each layer's scriptural foundation — anchored in the broadcast metaphor of Isaiah 30:21 and the Jeremiah 17 contrast. |
| [Reading List](https://syncshepherd-main.github.io/garys-garden/reading-list.html) | `recommended-reading.md` | Complete bibliography for both frameworks — primary sources, supplementary reading, and a guided reading pathway. |

---

## Technical Details

- **Hosting:** GitHub Pages via GitHub Actions (auto-deploys on push to `main`)
- **Stack:** Pure static HTML/CSS/JS — no build tools, no frameworks, no dependencies
- **Fonts:** Google Fonts (Inter)
- **Markdown rendering:** Custom client-side parser in each source document page (fetches `.md` files and renders to HTML)
- **Responsive:** Hamburger menu on mobile (< 700px breakpoint), fluid card grid on homepage

## File Structure

```
garys-garden/
  index.html                    Homepage — card grid linking to all pages
  7-tier-framework.html         Interactive 7-tier viewer (sidebar nav, JS renderers)
  holistic-recovery-model.html  Interactive 8-layer recovery viewer (sidebar nav, JS renderers)
  7-tier-full-text.html         Renders 7-Tier-Framework.md
  eight-layer-reference.html    Renders seven-layers.md
  biblical-roots-doc.html       Renders biblical-roots.md
  reading-list.html             Renders recommended-reading.md
  7-Tier-Framework.md           Source: 7-tier relational framework
  seven-layers.md               Source: 8-layer recovery model
  biblical-roots.md             Source: biblical roots theological supplement
  recommended-reading.md        Source: bibliography and reading list
  .github/workflows/static.yml  GitHub Pages deployment workflow
```

## License

This work is offered freely. No rights reserved.
