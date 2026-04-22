# 🪵 Lily's MakerSpace Portfolio

A warm, handcrafted personal portfolio showcasing laser cutting, 3D printing, woodworking, electronics, and DIY projects made at Northeastern's MakerSpace.

**Live site:** `https://lilyntran98.github.io/makerspace-portfolio`

---

## 📁 Folder Structure

```
makerspace-portfolio/
├── index.html
├── README.md
└── images/
    ├── photo1.jpg           ← About section portrait
    ├── IMG_1769.jpg         ← Wooden speaker
    ├── IMG_2222.jpg         ← Engraved glass cup
    ├── IMG_3733.jpg         ← 3D printed phone holder
    ├── IMG_4222.jpg         ← Microfluidic device
    ├── IMG_4256.jpg         ← Wooden laundry hanger
    ├── IMG_4748.jpg         ← Coasters in progress
    ├── IMG_4757.jpg         ← Finished wooden coasters
    ├── IMG_4758.jpg         ← Wooden charcuterie board
    ├── IMG_4761.jpg         ← Finished wooden coasters (alt)
    ├── IMG_5082.jpg         ← Digital clock (front)
    ├── IMG_5083.jpg         ← Digital clock (back)
    ├── IMG_5431.jpg         ← Cat wooden coaster
    ├── IMG_5432.jpg         ← Wooden lantern
    └── IMG_5735.jpg         ← Engraved wooden box
```

---

## ➕ How to Add a New Project

Copy and paste this template inside the `<div id="projectsGrid">` section of `index.html`:

```html
<article class="project-card" data-category="laser"
  onclick="openLightbox(
    'Your Project Title',
    'Laser Cutting',
    'A description of your project — what it is, how you made it, and why.',
    'Tools used (e.g. Epilog Laser · Inkscape)',
    'Northeastern MakerSpace',
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
    <p class="project-meta">Material · MakerSpace</p>
  </div>
</article>
```

**For `data-category`**, use one of:
- `laser` → Laser Cutting filter
- `3d` → 3D Printing filter
- `wood` → Woodworking filter
- `electronics` → Electronics filter

---

## 🎨 Quick Customizations

| What | Where in index.html |
|------|---------------------|
| Name in nav | `Lily Lee — MakerSpace` |
| Hero title / subtitle | Hero section, ~line 190 |
| About me paragraphs | About strip section, ~line 295 |
| Skill chips | Below about text, ~line 310 |
| Process steps | Process section, ~line 340 |
| Footer GitHub link | Bottom of file |

---

## 📸 Photo Tips

- Keep photos under **1MB** for smooth GitHub uploads (use [squoosh.app](https://squoosh.app) to compress)
- **No spaces in filenames** — use `photo1.jpg` not `photo 1.jpg`
- Landscape photos (4:3 ratio) work best for project cards
- Square photos work best for the About portrait

---

Made with ♥ at Northeastern MakerSpace
