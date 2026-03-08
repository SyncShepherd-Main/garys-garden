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

### Reference & Study

| Page | Description |
|------|-------------|
| [Recommended Reading](https://syncshepherd-main.github.io/garys-garden/recommended-reading.html) | A complete bibliography for the Eight-Layer Recovery Model, the 7-Tier Framework, and the Gospel foundation — including a curated reading pathway. Interactive sidebar with 30+ books. |
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

## Technical Details

- **Hosting:** GitHub Pages via GitHub Actions (auto-deploys on push to `main`)
- **Stack:** Pure static HTML/CSS/JS — no build tools, no frameworks, no dependencies
- **Font:** EB Garamond (Google Fonts), fallback: Georgia, serif
- **Body text:** 18px, line-height 1.85
- **Markdown rendering:** Custom client-side `parseMarkdown()` in each source document page (fetches `.md` files and renders to HTML)
- **Responsive:** Hamburger menu on mobile (< 700px breakpoint), fluid card grid on homepage, sidebar collapses on mobile (< 720px)

## File Structure

```
garys-garden/
  index.html                    Homepage — card grid linking to all pages
  7-tier-framework.html         Interactive 7-tier viewer (sidebar nav, JS renderers)
  holistic-recovery-model.html  Interactive 8-layer recovery viewer (sidebar nav, JS renderers)
  biblical-roots-doc.html       Biblical roots interactive viewer (hardcoded content)
  immanuel-moments.html         Immanuel Moments testimony (hardcoded content)
  recommended-reading.html      Recommended reading interactive viewer (sidebar nav)
  paul-essay.html               Paul essay viewer (renders paul-and-the-old-testament.md)
  7-tier-full-text.html         Source viewer (renders 7-Tier-Framework.md)
  eight-layer-reference.html    Source viewer (renders seven-layers.md)
  biblical-roots-source.html    Source viewer (renders biblical-roots.md)
  immanuel-moments-source.html  Source viewer (renders immanuel-moments.md)
  7-tier-flowchart-view.html    Flowchart image viewer with navigation
  7-tier-flowchart.png          Visual flowchart of the 7-tier framework
  7-Tier-Framework.md           Source: 7-tier relational framework
  seven-layers.md               Source: 8-layer recovery model
  biblical-roots.md             Source: biblical roots theological supplement
  immanuel-moments.md           Source: Immanuel Moments testimony
  paul-and-the-old-testament.md Source: Paul & the Old Testament essay
  recommended-reading.md        Source: bibliography and reading list
  .github/workflows/static.yml  GitHub Pages deployment workflow
```

## License

This work is offered freely. No rights reserved.
