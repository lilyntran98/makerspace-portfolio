# Lily's MakerSpace Portfolio

A warm, handcrafted personal portfolio site showcasing laser cutting, 3D printing, woodworking, and DIY craft projects made at Northeastern's MakerSpace.

**Live site:** `https://lilyntran98.github.io/makerspace-portfolio`

---

## 📁 Folder Structure

Set up your repo like this:

```
makerspace-portfolio/
├── index.html          ← the portfolio (already done!)
├── README.md           ← this file
└── images/             ← put ALL your photos here
    ├── hero1.jpg
    ├── hero2.jpg
    ├── hero3.jpg
    ├── hero4.jpg
    ├── portrait.jpg
    ├── project-box.jpg
    ├── project-planter.jpg
    └── ...
```

---

## 🖼️ How to Add Your Photos

### Hero section (top 4 photos)

Find this block in `index.html` (around line 200) and replace each placeholder `<div>` with an `<img>` tag:

```html
<!-- BEFORE (placeholder) -->
<div class="hero-grid-cell placeholder">
  <span class="ph-icon">🪵</span>
  <span>Add photo</span>
</div>

<!-- AFTER (your photo) -->
<div class="hero-grid-cell">
  <img src="images/hero1.jpg" alt="My laser cut project"/>
</div>
```

### Portrait photo

Find the `about-portrait` div (around line 290) and replace the placeholder:

```html
<!-- BEFORE -->
<span class="about-portrait-ph">🪴</span>

<!-- AFTER -->
<img src="images/portrait.jpg" alt="Lily Lee"/>
```

### Project card photos

Each project card has a `project-thumb` div. Replace the placeholder emoji span with an img tag:

```html
<!-- BEFORE -->
<div class="project-thumb">
  <span class="ph-big">🔆</span>
</div>

<!-- AFTER -->
<div class="project-thumb">
  <img src="images/project-box.jpg" alt="Engraved Keepsake Box"/>
</div>
```

Also update the `onclick` on the card — the last parameter is the lightbox image path:

```html
<!-- Find the onclick and update the last "" to your image path -->
onclick="openLightbox('Engraved Keepsake Box', 'laser', '...desc...', '...tools...', 'Spring 2025', 'Birch plywood', 'images/project-box.jpg')"
```

---

## ➕ How to Add a New Project Card

Copy and paste this template inside the `<div id="projectsGrid">` section:

```html
<article class="project-card" data-category="laser"
  onclick="openLightbox(
    'Your Project Title',
    'Laser Cutting',
    'A description of your project — what it is, how you made it, and why.',
    'Tools used (e.g. Epilog Laser · Inkscape)',
    'Season Year',
    'Materials used',
    'images/your-photo.jpg'
  )">
  <div class="project-thumb">
    <img src="images/your-photo.jpg" alt="Your Project Title"/>
  </div>
  <div class="project-info">
    <span class="project-tag">Laser Cutting</span>
    <h3 class="project-name">Your Project Title</h3>
    <p class="project-desc">Short one-liner description for the card.</p>
    <p class="project-meta">Material · Season Year</p>
  </div>
</article>
```

**For `data-category`**, use one of:
- `laser` → shows under "Laser Cutting" filter
- `3d` → shows under "3D Printing" filter
- `wood` → shows under "Woodworking" filter
- `craft` → shows under "DIY Crafts" filter

---


### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, choose **Deploy from a branch**
3. Select branch: `main`, folder: `/ (root)`
4. Click **Save**

Your site will be live at:
```
https://YOUR-USERNAME.github.io/makerspace-portfolio
```
(It may take 1–2 minutes to appear the first time.)

### Step 4 — Update the footer link

In `index.html`, find this line near the bottom and replace the GitHub URL:

```html
<a href="https://github.com/YOUR-USERNAME/makerspace-portfolio" target="_blank">GitHub</a>
```

---

## 🎨 Customizations

| What | Where in index.html |
|------|---------------------|
| Your name in the nav | Line ~170: `Lily Lee — MakerSpace` |
| Hero title / subtitle | Lines ~190–200 |
| About me paragraph | Lines ~295–305 |
| Skill chips | Lines ~310–320 |
| Footer email link | Near bottom: `mailto:...` |
| Process steps text | Lines ~340–380 |

---

## 📸 Photo Tips

- **Recommended size:** 1200×900px or larger (landscape) for project cards
- **Portrait photo:** 800×800px (square) works best
- **Format:** `.jpg` (smaller file size) or `.png`
- **File names:** use lowercase, no spaces — e.g. `laser-box.jpg` not `Laser Box Photo (1).jpg`

---

Made with ♥ at Northeastern MakerSpace
