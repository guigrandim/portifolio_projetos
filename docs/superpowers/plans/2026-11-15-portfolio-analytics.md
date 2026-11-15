# Portfolio Analytics Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Redesign the static portfolio to attract analytics clients and make Guilherme's Data Science and Analytics expertise clear.

**Architecture:** Keep the site static and preserve its existing GitHub Pages links. Use the Stitch screen as the visual source, adapt its structure and palette in `index.html` and local CSS in `assets/css/custom.css`, and retain local portfolio content and assets without adding runtime dependencies.

**Tech Stack:** HTML5, CSS, existing JavaScript and static assets.

**Spec:** `docs/superpowers/specs/2026-11-15-portfolio-analytics-design.md`

## Global Constraints

- The page remains static in HTML, CSS, and JavaScript.
- Keep current project, contact, and social destinations working.
- Use only metrics and claims already documented in the current portfolio.
- Label the R$ 492 million figure as potential savings estimated by the procurement analysis.
- Deliver the executable redesign in this repository; use the existing Stitch and Figma artifacts as the design source.
- Do not add frameworks, a backend, a CMS, or runtime dependencies.
- Keep the page responsive, keyboard accessible, and respectful of `prefers-reduced-motion`.

## Review Focus

- Unsupported numeric claims: review all displayed figures against the existing case copy, especially the estimated R$ 492 million potential savings.
- Contact and project URLs: preserve `mailto:gui.grandim@gmail.com`, WhatsApp, social, GitHub, and demo destinations.
- Small screens: inspect the compact navigation, metric panel, case grid, and contact section for overflow and readable line lengths.
- Keyboard access: check visible focus on navigation, CTAs, and project links.
- Motion preferences: confirm content remains understandable with reduced motion enabled.

---

### Task 1: Rebuild the page content around the client journey

**Files:**
- Modify: `index.html`

**Interfaces:**
- Produces section anchors consumed by the page navigation: `#services`, `#cases`, `#about`, and `#contact`.
- Produces CSS hooks: `.site-header`, `.section-inner`, `.hero-layout`, `.evidence-panel`, `.service-list`, `.case-study`, and `.contact-grid`.
- Uses semantic `header`, `nav`, `main#page-content`, section, and `footer` elements.
- Preserves all existing contact, social, project repository, and demo URLs.

- [x] **Step 1: Implement Stitch navigation** as a fixed desktop sidebar and compact mobile header with links to Início, Serviços, Cases, Habilidades, Sobre, and Contato plus a clear contact CTA; keep semantic `header`, `nav`, `main#page-content`, sections, and `footer` elements.
- [x] **Step 2: Rewrite the hero copy** with the headline “Transformo dados em decisões que movem o negócio.”, a short description of the analytics offer, a “Vamos conversar” CTA, and a “Ver cases” anchor link; place the content in `.section-inner` and `.hero-layout` wrappers.
- [x] **Step 3: Add a data-backed evidence panel** with the `.evidence-panel` hook for the public procurement case: show 164,680 records, four hypotheses tested, and “R$ 492 milhões em economia potencial estimada”; label the metric as potential, not realized savings. Represent the API → consolidated dataset → forecast flow without drawing a fabricated time series.
- [x] **Step 4: Add three client-facing service summaries** for Analytics e BI, Análise e modelagem preditiva, and Produtos e pipelines de dados inside `.service-list`, with tooling mentioned only as supporting detail.
- [x] **Step 5: Present all seven `.case-study` projects** (public procurement, Rossmann, SRAG, video games, coffee sales, Curry deliveries, and ML experiments), retaining their local images, stacks, factual caveats, and existing GitHub or demo links.
- [x] **Step 6: Condense About and Skills** into the UNICAMP and USP credentials, sports analytics experience, and capability groups; use `.section-inner` for section width and retain the SRAG model limitation if that project is referenced.
- [x] **Step 7: Keep the contact section focused** in `.contact-grid` on the existing email and WhatsApp links, with LinkedIn and GitHub as secondary paths. Update title, description, and social metadata to match the Portuguese positioning.

**Manual check:** Review the markup and destinations in `index.html`; confirm every metric and URL matches the current portfolio.

### Task 2: Apply the new visual system and responsive layout

**Files:**
- Modify: `assets/css/custom.css`
- Create: `assets/webfonts/space-grotesk-variable.woff2`
- Create: `assets/webfonts/ibm-plex-sans-variable.woff2`
- Create: `assets/webfonts/SpaceGrotesk-OFL.txt`
- Create: `assets/webfonts/IBMPlexSans-OFL.txt`

**Interfaces:**
- Consumes: the section anchors and component classes introduced in Task 1.
- Produces: responsive visual styles for navigation, hero, evidence panel, services, case studies, About, and Contact.

- [x] **Step 1: Define the Stitch CSS tokens** for background `#0A0E14`, surfaces `#0E131A` and `#141922`, cyan `#22D3EE`, orange `#F97316`, text `#F1F5F9`, and muted text `#94A3B8`.
- [x] **Step 2: Add local font assets and their SIL Open Font License texts** under `assets/webfonts/`; source Space Grotesk and IBM Plex Sans from their official Google Fonts repositories.
- [x] **Step 3: Define `@font-face` and establish the editorial type scale** with local Space Grotesk for headings and IBM Plex Sans for body copy, plus system fallbacks.
- [x] **Step 4: Replace the previous light theme in `custom.css`** with Stitch's dark technical visual system: desktop sidebar, compact mobile navigation, glass-like surfaces, and cyan/orange accents; leave the compiled `main.css` and existing `main.js` untouched.
- [x] **Step 5: Style the hero as a two-column composition** with the offer on the left and the procurement evidence panel on the right; make the panel stack below the headline on narrow screens.
- [x] **Step 6: Style services, technology groups, and all seven cases** using the Stitch card and panel language; use the real local project illustrations and distinguish the featured procurement case.
- [x] **Step 7: Add small-screen layout rules** at the existing project breakpoints so navigation, text, evidence, and case content stack without horizontal overflow.
- [x] **Step 8: Add visible `:focus-visible` treatment and reduced-motion rules**; ensure color contrast keeps body text and links readable on both light and slate sections.

**Manual check:** Inspect the CSS cascade to ensure the custom rules override the template without editing `assets/css/main.css`.

### Task 3: Review the page in a browser

**Files:**
- Review: `index.html`
- Review: `assets/css/custom.css`

- [ ] **Step 1: Open the static page at desktop width** and review hierarchy, spacing, typography, evidence-panel legibility, and case order.
- [ ] **Step 2: Review at mobile width** and confirm the navigation, CTA, evidence panel, and project cards fit without horizontal scrolling.
- [ ] **Step 3: Navigate with the keyboard** and confirm all links are reachable and show focus.
- [ ] **Step 4: Enable reduced motion** and confirm no essential content depends on animation.
- [ ] **Step 5: Follow the main contact, repository, and demo links** to confirm their destinations remain the ones present in the current portfolio.

**Review note:** The local browser preview could not be opened in this session (browser access host unavailable; Chrome window minimized). No browser or test-suite verification is claimed.
