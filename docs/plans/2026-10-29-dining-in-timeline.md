# Dining in Timeline Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Move all meal candidates into their matching timeline entries and add evening breakfast-supply options without disturbing the route grid.

**Architecture:** Keep the existing static HTML and vanilla JavaScript. Replace the standalone dining section with compact horizontal pick tracks inside the Saturday and Sunday meal entries, then reuse the same interaction for breakfast procurement.

**Tech Stack:** HTML, CSS, vanilla JavaScript, local image assets.

---

### Task 1: Add local image assets

**Files:**
- Create: `trip-final-assets/restaurants/*.jpg`

**Step 1:** Download the verified Amap review images for missing restaurants and breakfast shops.

**Step 2:** Confirm each file is a valid JPEG and not an HTML error page.

### Task 2: Move dining content into the timeline

**Files:**
- Modify: `index.html`

**Step 1:** Remove the standalone `#dining` navigation item and section.

**Step 2:** Add compact horizontal pick tracks to Saturday lunch, Saturday dinner, and Sunday lunch.

**Step 3:** Add three breakfast-procurement options to the Saturday evening preparation entry.

**Step 4:** Keep the transport route grid, its images, and its 2x2 layout unchanged.

### Task 3: Verify the local preview

**Files:**
- Modify: `D:\codex\trip-final-2026-10-31.html`
- Modify: `D:\codex\trip-final-assets\restaurants\*`

**Step 1:** Sync the repository preview files to the root preview paths.

**Step 2:** Open the page in local Chrome and check desktop and mobile widths.

**Step 3:** Confirm all images load, each meal track scrolls, no page-level horizontal overflow appears, and the route grid remains 2x2.

**Step 4:** Stop before commit and push so the user can review the local preview.
