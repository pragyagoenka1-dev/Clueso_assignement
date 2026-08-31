# Clueprint — interactive product demo

An interactive, single-file prototype of **Clueprint**, a reusable video-blueprint feature
concept for [Clueso](https://clueso.io) (turns screen recordings into polished product videos).

A Clueprint captures an existing video (or a prompt) as a template with **fixed parts** and
**variable slots**, so teammates can spin up new on-brand videos in minutes.

## Run it

No build, no dependencies (fonts load from Google Fonts). Either:

- Open `index.html` directly in a browser, or
- Serve the folder: `npx serve .` / `python -m http.server`

Hosted on **GitHub Pages**: enable Pages on this repo (Settings → Pages → deploy from
branch, root) and the demo is live at your Pages URL.

## The flow

1. **Templates** — create a Clueprint from the dashed card or the "New Clueprint" button
2. **Path chooser** — start from a Clueso video (recommended), an uploaded reference, or a prompt
3. **Analyze** — a laser film-scanner reads structure, pacing, branding, and reusable slots
4. **Review** — two-column editor: live preview + scene timeline on the left; agent
   instructions, editable scenes, timing, branding, text styles, and variable slots on the right.
   The **lock / variable toggle** is the core interaction: locked = fixed in the template,
   unlocked = filled in per video
5. **Video editor** — the saved Clueprint loaded in the Clueso editor, with a Publish
   split-button, slot-highlighted transcript, and a per-element Inspect panel where every
   property (position, size, typography) carries its own template lock

**Tip:** hit **Play demo** (bottom-left) for a ghost-cursor auto-walkthrough of all three
creation paths, or **Reset** to restore the initial state.

## Design tokens

- Font: Geist / Geist Mono
- Accent: `#DA5CC7` (used sparingly)
- Dark palette: bg `#0a0a0b`, panels `#141416 / #1a1a1d / #202024`, lines `#2a2a2e / #212125`
- Radii: 14 (cards/modals), 9 (buttons), 7 (chips)

Everything lives in `index.html` — markup, styles, and state — so the whole prototype is
one portable file.
