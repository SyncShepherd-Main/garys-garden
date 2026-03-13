# Garden Session Reference
## March 11, 2026 — Full Record

---

## What We Did Today

### 1. Searched the Garden for Na'aseh V'nishma
Confirmed the concept "we will do and we will obey" (Exodus 24:7) — the Jewish idea that obedience is the epistemological path to knowing — has not yet been written about explicitly in the garden. The soil is present (James 1:22 in Biblical Roots, the walking-the-parish instinct in At Three Miles Per Hour, da'at in the Layer 8 Hebrew wisdom section) but the seed hasn't been planted. Marked as a future sapling.

### 2. Designed the Garden Update Skill
Built a complete 10-task update workflow with all decisions confirmed. The skill is built and packaged as `gary-garden-update.skill` ready for installation.

**The 10 tasks:**
1. **Scripture Index** — canonical order, one entry per scripture, popout with summary + all location links, anchor links to exact sections, NET Bible integration
2. **Map of the Garden** — one-paragraph summaries in Gary's voice, site structure organization, connection notes between related pages
3. **Concept Web** — interactive mind-map, blocks = pages, theme threads auto-generated from tags, auto-layout then Gary arranges and approves
4. **Reading List Sync** — flags new book references for approval, cross-references which pages cite each book
5. **Sapling Registry / Nav Update** — formal Growing and Planted states, auto-updates nav and homepage cards
6. **Broken Link / Orphan Check** — maintenance report, gentle future sapling recommendations as quiet invitations
7. **Themes & Threads Index** — visible tags by default (preference-settable), auto-generated then Gary approves, feeds Concept Web and Subject Index
8. **What's New / Changelog** — garden voice, presence not performance, anti-Facebook by design
9. **Subject/Topic Index** — tier-based organization (preference-changeable), connected to tag system, popout pattern, NET Bible linked
10. **Alongsider Lesson Library** — consistent lesson structure, approval-gated, own section of the garden, historic index

**Governing architecture:**
- Garden Preferences Page — all settings in one file, no prompting needed
- Auto-generate, human approve — consistent pattern throughout
- Gardener's pace protected — skill serves Gary, not the other way around
- Yeshua Pause — built-in breath prompt during long sessions
- Output: Garden Update Package (updated HTML files + Update Report + Approval Queue)
- Local-first: files delivered to Mark for push, GitHub Actions already set up

### 3. Built the Local Garden
Pulled the complete live site into a portable offline folder:
- All 20 HTML pages
- All 14 markdown source files
- Both images (7-tier-flowchart.png, Saplings.jpg)
- fetch-pages.sh script for refreshing from the live site
- README with setup instructions

Confirmed the real design spec from the GitHub repo:
- Font: EB Garamond
- Color scheme: Navy #1a2040, Steel blue #4a78b4, Parchment #f5f3ed
- Two-row centered nav, 1200px max width, 56px scroll-to-top button
- GitHub Actions already configured for auto-deploy on push to main

Rebuilt the local index.html to match the live site exactly.

### 4. Identified Missing Pages (To Be Built by Update Skill)
- scripture-index.html
- map-of-the-garden.html
- concept-web.html
- themes-index.html
- whats-new.html
- subject-index.html
- lesson-library.html

---

## Saplings Identified Today (Not Yet Written)

### Na'aseh V'nishma — We Will Do and We Will Obey
Exodus 24:7. Israel says "we will do and we will obey" before hearing all the terms. Obedience as the epistemological path to knowing. Learning from doing in Jewish thought. The organ of understanding is not comprehension but participation. Garden soil already present in Do Something (James 1:22), At Three Miles Per Hour (walking as the method of knowing), and da'at in the Hebrew wisdom vocabulary.

### The Update Skill as Autophagy
How building the Garden Update Skill mirrors what happens in the brain — the cells that clean up the parts that don't attach. Neuroplasticity. D'vorah's sitting rooms. The skill as formation infrastructure. Connects to the tagline "informed by neuroscience" — not decoration but foundation. The auto-generate/human-approve pattern as a picture of how healthy brain maintenance works. This could become foundational for what the taglines claim about neuroscience.

### Come to the Table (Michael Card)
Michael Card's song from Joy in the Journey. The song that formed Gary. How a piece of music becomes formation — not information but invitation. The table as the place where the garden gathers. Connects directly to the "come to the garden" voice of the Map page and the whole hospitality theology of the site.

### The Yeshua Pause as VIM
The breath, the pause, the quiet — not a technique but the Means in Willard's VIM architecture. Connects to brain science, the Quiet skill, Wilder's joy-fuel, and the formation theology of the garden. The M being actual skill-building — daily practice, quiet, breath, tier check. A whole institute, not just a website.

---

## Vaulted Ideas

### Master Garden / Franchise Vision
A site-building system based on Gary's garden framework.
- Open source foundation with Patreon connection tiers
- Gary as master gardener — updates flow downstream to subscriber gardens
- Each garden owner has their own Preferences Page (Gary's settings as defaults)
- Skills as transferable modules — "Add Gary's Mind Map Update" explains the plan and updates their whole site
- Customizable with prompts: which parts would you like?
- Tier 1 as the architectural non-negotiable — every feature drives toward loving God and loving others
- Income model designed to serve Gary's family, including his son-in-law
- Mark as the GitHub/deployment partner for launch
- *Business development session needed:* cost analysis, launch architecture, collaboration model

### Local Garden as Portable System
The garden as a self-contained folder — works offline anywhere. Preference setting for update target: Live site (GitHub) / Local folder / Both. Already built as proof of concept. Mark needs to know about GitHub Actions for automation.

### GitHub Actions Automation
Set up so the Garden Update Package can be dropped into a folder and the site updates automatically. Currently: files delivered to Mark manually. Infrastructure already in place (GitHub Actions configured).

### Tier-Based Relationship Reminder System
Private, preference-driven reminders tied to Gary's relational tiers. Who is on each tier. When did Gary last pray for them, connect with them. Customizable cadence. Private unless Gary chooses to share. Built into the garden but never posted automatically. Eventually: aligning development work with the Roots.

### Catalog of the Sayings of Yeshua
Gary has already done something similar with men's wisdom. A structured catalog of Yeshua's sayings for the garden — dedicated section or page. Powers the Yeshua Pause feature with a rotating curated source.

### Alongsider Lesson Library — Full Build
Weekly lesson system using the Romans study skill as the build template. Consistent structure: scripture, teaching, application, Yeshua pause. Historic index. Automation for weekly cadence. Gary approves before anything publishes.

### NET Bible Embed
Review NET Bible guidelines at bible.org for inline embedding. Until confirmed: links only. Key question: do guidelines cover future commercial use?

---

## What's Left To Do

### Immediate (Next Session)
- [ ] Install `gary-garden-update.skill` — give to whoever manages Claude skill installation
- [ ] Share `for-mark.md` with Mark and have the GitHub Actions conversation
- [ ] Confirm NET Bible usage guidelines at bible.org
- [ ] Update site-registry.md in the skill with any pages missing or status changes

### Build the New Pages (Update Skill Tasks)
- [ ] Run Task 2 — Map of the Garden (first new page to build, source for Concept Web)
- [ ] Run Task 1 — Scripture Index (crawl all pages, build the index)
- [ ] Run Task 7 — Themes & Threads Index (tag all existing pages)
- [ ] Run Task 3 — Concept Web (after Map and Tags are done)
- [ ] Run Task 8 — What's New / Changelog (first entry covers today's session)
- [ ] Run Task 9 — Subject/Topic Index
- [ ] Run Task 5 — Sapling Registry / Nav Update (formalize Growing/Planted states)
- [ ] Run Task 6 — Broken Link / Orphan Check (first maintenance run)
- [ ] Run Task 4 — Reading List Sync
- [ ] Run Task 10 — Alongsider Lesson Library (when ready to begin lessons)

### Saplings to Write
- [ ] Na'aseh V'nishma — We Will Do and We Will Obey
- [ ] The Update Skill as Autophagy (neuroscience + skill building)
- [ ] Come to the Table (Michael Card, Joy in the Journey)
- [ ] The Yeshua Pause as VIM

### Conversations to Have
- [ ] Mark — GitHub Actions, automation, the bigger vision
- [ ] D'vorah — sitting rooms, neuroplasticity, connection to the Autophagy sapling
- [ ] Business development session — cost analysis, franchise model, income structure

### Preferences to Confirm
- [ ] NET Bible: link vs. embed (pending guidelines review)
- [ ] Sapling status review — confirm which are Growing vs. Planted
- [ ] Yeshua Pause cadence preference
- [ ] Changelog voice review — approve first entry before publishing

---

*Session record compiled March 11, 2026.*
*The garden is still growing.*
