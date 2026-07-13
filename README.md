# InvictusGameStudioEditor

Rodrigo Giliberti's portfolio site — a single self-editing page (`index.html`).

## Files
```
/
├── index.html       — The whole site: title, subtitle, 3 category boxes
│                       (Game Design / Level Design / My Games), and a
│                       Contact / Social / Resume row. Clicking a box opens
│                       an in-page panel — no separate pages, no reload.
├── site-data.json    — Admin edits (text, galleries, box images, social
│                       links), committed here so other visitors see changes
├── resume.pdf        — Resume PDF linked from the Resume box
├── project.html      — Legacy per-project case-study template (unused by
│                       the current home page, kept in case it's wanted later)
├── projects.json     — Legacy project list used only by project.html
└── images/site/      — Screenshots referenced by site-data.json
```

## Admin Password
Default: `rg2025admin`

**To change it:** open `index.html`, find `const ADMIN_HASH = '...'` and
replace it with the SHA-256 hash of your new password.

## Editing the site
1. Click the lock icon (bottom-right) and log in — the admin bar appears.
2. **Edit Texts** / **Edit Images** / **Skill Bars** / **Layout** toggle what
   you can click-and-change on the page (box labels, panel content, bios,
   timeline, contact info, gallery images, positions).
3. **Save & Download** → downloads `site-data.json`. Commit it (and any new
   images under `images/site/`) to this repo so the changes go live for
   every visitor.

## Deploy
GitHub Pages → Settings → Pages → Branch: main → / (root).
