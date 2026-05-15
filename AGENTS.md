# Agent Collaboration Guide

This repository is shared between the user, Codex, and Claude Desktop. Treat this file as the coordination layer for agentic workflows so work stays understandable across tools.

## Source of Truth

- The shared workspace is `G:\My Drive\AI\GitHub\Portfolio\Professional Portfolio`.
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
- Supporting pages include `about.html`, `bone-printer.html`, `fpv-drone.html`, `thermofisher.html`, `automated-desk.html`, and `robotics.html`.
- Current README: "Portfolio site showcasing all my projects."

## Current Task State

Status: Ready for coordinated work.

Owner: User / next active agent.

Last updated: 2026-05-15 by Codex.

Recent changes:

- Added this `AGENTS.md` file as the shared handoff and workflow guide.

Open questions:

- None.

Next steps:

- Before making portfolio edits, update this section with the active task and intended files.
