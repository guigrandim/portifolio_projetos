# Airbnb Price Project 09 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add Airbnb Price to the static portfolio as project 09 with its existing image, links, and clearly qualified projected economic impact.

**Architecture:** Extend the existing `.case-study` list in `index.html` with one card after the current cases. Reuse the current HTML structure and local image; no CSS, JavaScript, dependency, or asset-generation changes are needed.

**Tech Stack:** Static HTML and existing local PNG asset.

**Spec:** `docs/superpowers/specs/2026-11-15-airbnb-price-project-09.md`

## Global Constraints

- Use `images/projeto09.png` and mark the case as project 09.
- Present `+€ 2,05 milhões (+1,75%)` as projected annual gross booking volume, not realized profit or ROI.
- State that the scenario holds estimated nights constant and compares the announced prices with model references across 20.026 listings.
- State that the snapshot is from December 2018 and percentage ROI was not calculated because incremental platform revenue and project costs are unavailable.
- Include the documented historical model metrics and the GitHub and Streamlit links.
- Use the exact Portuguese card copy and stack recorded in the spec.
- Keep the site static and reuse its existing case-card markup.

## Review Focus

- The headline metric must read as projected gross booking volume, not as realized savings or ROI.
- The caveat must explain the missing revenue and cost inputs needed to calculate ROI.
- The December 2018 data date must stay visible with the historical projection.
- Both external destinations and the local image path must match the project README and workspace.
- The new card must use the established `.case-study` structure and project number 09.

---

### Task 1: Add the Airbnb Price case

**Files:**
- Modify: `index.html` in the `#cases` `.case-list`
- Use: `images/projeto09.png`

**Interfaces:**
- Consumes: the existing `.case-study`, `.case-meta`, `.case-visual`, `.case-content`, `.case-result`, `.stack-list`, and `.case-links` styles and markup.
- Produces: one project 09 card with a locally loaded illustration, business summary, projected volume result and caveat, model metrics, stack, repository link, and live app link.

- [x] Append one `.case-study` article after the current final case. Set its number to `09`, use the alt text “Ilustração do simulador de comparação de diárias para Amsterdam”, and copy the title, summary, result, caveat, model metrics, stack, and links exactly from the spec. Keep `+€ 2,05 milhões (+1,75%)` identified as projected annual gross booking volume.
