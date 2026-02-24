# Rodrigo Giliberti — Portfolio v3

## Files
```
/
├── index.html          ← Main portfolio (hero, about, projects, etc.)
├── project.html        ← Case study template (auto-loads by ?id=0, ?id=1, etc.)
├── projects.json       ← Project data — edit via admin or manually
├── resume.pdf          ← ⚠ ADD THIS: your resume PDF
└── images/
    └── projects/       ← ⚠ ADD project screenshots here
        ├── endless-skies.jpg
        └── ...
```

---

## Admin Password
Default: `rg2025admin`

**To change it:** open both `index.html` and `project.html`,
find the line that says `const ADMIN_PASS = 'rg2025admin';` and replace it.

---

## How to use the Admin

### On index.html:
1. Click the **lock icon** (bottom-right corner)
2. Enter your password → admin bar appears at the top
3. Use the toolbar:
   - **Edit Texts** → click any text on the page to edit inline
   - **Edit Images** → click any project thumbnail to upload a new image
   - **Skill Bars** → drag the bars left/right to adjust percentages
   - **Reorder** → drag projects up/down to reorder them
   - **+ Add Project** → adds a new blank project
4. Click **Save & Download** → downloads `projects.json`
5. Upload that file to your GitHub repo → site updates in 30s

### On project.html:
- Same login session carries over (same tab/browser)
- **Edit Texts** → click any section text to edit
- **Edit Images** → click hero image or gallery slots to upload
- **Save & Download** → downloads `project-0-content.json` (or whatever id)
- Upload that too if you want it persistent across devices (optional — localStorage works locally)

---

## Deploy to GitHub Pages

1. Create repo: `rodrigogiliberti.github.io`
2. Upload all files to root
3. Settings → Pages → Branch: main → / (root) → Save
4. Site live at: `https://rodrigogiliberti.github.io`

### Adding images:
- Put project screenshots in `images/projects/`
- Name them clearly: `endless-skies-1.jpg`, `myproject-blockout.jpg`
- In the admin, set the image path to `images/projects/your-file.jpg`

### Updating projects.json on GitHub:
- Admin → Save & Download → get `projects.json`
- Go to your GitHub repo → click `projects.json` → Edit → paste content → Commit

---

## Timeline (About section)
Edit directly in `index.html` — search for `exp_2_year`, `exp_2_title`, `exp_2_desc`
and update with your real history.
