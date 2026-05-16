# Agent Collaboration Guide

This repository is shared between the user, Codex, and Claude Desktop. Treat this file as the coordination layer for agentic workflows so work stays understandable across tools.

## Source of Truth

- The shared workspace is `G:\My Drive\Projects\AI\GitHub\Portfolio\HTML Files`.
- Files in this repository are the source of truth. Chat history in any one app is not shared unless it is written here.
- Before making edits, inspect the current files you plan to touch.
- Do not overwrite changes you did not make. If a file changed unexpectedly, pause and reconcile the current file contents.
- Prefer small, focused changes that are easy for another agent or the user to review.

## Handoff Protocol

When starting work:

1. Read this file.
2. Check the current task state below.
3. Inspect the files relevant to the task.
4. Note any assumptions before making broad changes.

When finishing work:

1. Update the task state if the next agent needs context.
2. List changed files and the reason for each change.
3. Record any verification performed, such as opening pages, checking links, or running tests.
4. Leave clear next steps if the work is incomplete.

## Conflict Rules

- User edits always take priority.
- If Codex and Claude Desktop both touch the same file, compare the current file carefully and preserve both intended changes where possible.
- Do not revert, reset, or delete work unless the user explicitly asks.
- If a merge is ambiguous, ask the user before choosing one version over another.

## Project Notes

- This is a static professional portfolio site.
- Main entry point: `index.html`.
- Supporting pages include `about.html` and project detail pages in `projects/`: `bone-printer.html`, `fpv-drone.html`, `thermofisher.html`, `automated-desk.html`, and `robotics.html`.
- Current README: "Portfolio site showcasing all my projects."

## Current Task State

Status: Portfolio update in progress.

Owner: Codex / supervised by user.

Last updated: 2026-05-15 by Codex.

Recent changes:

- Added this `AGENTS.md` file as the shared handoff and workflow guide.
- Created deployable `images/` asset copy inside the GitHub Pages repo using lowercase kebab-case names.
- Moved project detail pages into `projects/` to match existing homepage links.
- Added `resume.pdf` copy so existing resume links resolve.
- Wired real images into homepage project cards, About headshot, and the first media slot on each project page.
- Replaced most project-page placeholders with real figures and captions for Bone Printer, FPV Drone, Automated Desk, Robotics, and many ThermoFisher sections.
- Polished media presentation with consistent image cards, caption styling, subtle hover treatment, homepage image overlays, and a desktop About headshot layout.
- Added a hover/focus Projects dropdown to the fixed header on all pages, linking directly to each project page.
- Replaced homepage placeholder-overlaid project thumbnails with CSS carousels using real project images; the old SVG placeholder art is hidden.
- Changed project-page media to contain full images instead of cropping them.
- Added full project artifact galleries and a homepage Portfolio Snapshot strip so all deployable images/media are referenced at least once.
- Verified local `href`, `src`, and CSS `url(...)` references; no missing local file references found.
- Removed the redundant homepage Portfolio Snapshot strip and redesigned Selected Projects into a mixed featured/grid layout with hover motion and explicit clickable project-image affordance.
- Replaced the homepage resume placeholder/hand-built preview with `images/resume-preview.png`, generated from `resume.pdf`; the resume PDF link remains unchanged.
- Updated homepage tagline to "designs, develops, delivers.", replaced the Targeting status cell with Location: Danbury, Connecticut and Role: Mechanical Engineer, and fixed the LinkedIn URL to the resume-listed profile.
- Cleaned mojibake/special-character artifacts across homepage, About, and project pages.
- Updated Bone 3D Printer page so the first project images show Michael standing next to the printer and the full CAD model, with CAD/process images moved prominently near the top.
- Reworked project-page content flow to better match the original Google Sites pages:
  - Bone 3D Printer now follows the archived source sequence: project overview, binder jetting process, Z-axis redesign, original/redesigned piston sleeve, outer sleeve iterations, piston head, and base plate/serviceability. The old dumped artifact gallery was removed.
  - FPV Drone now keeps the original flow around frame geometry, flight simulation, arm optimization, FEA iterations, acceleration check, and final assembly. The old generic artifact gallery was replaced with narrative image blocks.
  - Automated Desk now follows the archived source sequence: initial manual crank, torque/motor decision, first gearbox iteration, final helical gearbox, controller faceplate, desk interface, and motion test. The old generic artifact gallery was replaced with narrative image blocks.
  - Robotics now follows the archived source sequence: competition overview plus 2021-2022, 2020-2021, and 2019-2020 season sections. The old generic artifact gallery was replaced with narrative image blocks.
  - ThermoFisher had no matching archived source page in the local export; its duplicate bottom artifact gallery was removed so remaining images stay attached to individual co-op stories.

Open questions:

- Git CLI is not available on PATH in this shell, so commit/status verification will need Git availability resolved before final commit.
- 13 specific image placeholders remain on `projects/thermofisher.html`; broader ThermoFisher artifacts are represented in the new gallery, but those exact plot/defect/test-fixture visuals are not clearly identifiable in the current asset filenames.
- Browser visual QA through the Browser plugin and bundled Playwright remained blocked by the local Node/browser runtime failing to initialize.
- Chrome headless visual QA succeeded for desktop screenshots of updated Bone, FPV Drone, Automated Desk, and Robotics project pages. Mobile screenshot attempt was blocked by the app usage-limit approval gate before it could run.

Next steps:

- Next stage: run a mobile browser QA pass when tooling is available, tune any project-page spacing/cropping that appears on mobile, resolve/replace the remaining ThermoFisher placeholders if matching assets are identified, then prepare for user-approved commit.
