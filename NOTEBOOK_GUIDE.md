# 📓 Notebook Decoration Guide
## How Every Lesson Notebook is Structured

Copy this pattern for **every lesson** (L1 → L7, and all future phases).

---

## 🗂️ Cell Structure — Every Notebook Has These 8 Sections

```
Cell 1 ── BANNER          (Markdown)  ← Blue header with phase/lesson/time/date
Cell 2 ── OBJECTIVES      (Markdown)  ← Bullet list of learning goals + key functions table
Cell 3 ── SETUP           (Markdown)  ← "Setup & Imports" header
Cell 4 ── imports         (Code)      ← All imports + path config
Cell 5 ── section 1..N    (Code)      ← Lesson content, one section per concept
Cell 6 ── EXERCISE        (Markdown)  ← Yellow box with your hands-on task
Cell 7 ── exercise-code   (Code)      ← Blank/template code for the exercise
Cell 8 ── NOTES           (Markdown)  ← Fill-in table for your observations
Cell 9 ── TAKEAWAYS       (Markdown)  ← Green footer + prev/next navigation
```

---

## 🎨 Color System

| Element | Color | Used For |
|---|---|---|
| Banner bg | `#0D1B2A` → `#1565C0` | Phase 1 (blue) header |
| Info box | `#E3F2FD` + left border `#1565C0` | Lesson description |
| Exercise box | `#FFF9C4` + left border `#F9A825` | Hands-on task (yellow) |
| Takeaways | `#1B5E20` → `#2E7D32` | Green success footer |
| Code hint | `background:#1B5E20` inline | Code inside green box |

### Phase Color Mapping

| Phase | Banner Gradient | Box Color | Emoji |
|---|---|---|---|
| P1 Raster | `#0D1B2A → #1565C0` | `#E3F2FD` | 🔵 |
| P2 Classical ML | `#0D2A0D → #2E7D32` | `#E8F5E9` | 🟢 |
| P3 Deep Learning | `#1A0D2A → #6A1B9A` | `#F3E5F5` | 🟣 |
| P4A Segmentation | `#0D2A26 → #00695C` | `#E0F2F1` | 🩵 |
| P4D Agri Satellite | `#0D2A0D → #388E3C` | `#F1F8E9` | 🌾 |
| P4E UAV | `#2A1A0D → #E65100` | `#FFFDE7` | 🚁 |
| P4F Disease | `#2A0D18 → #880E4F` | `#FCE4EC` | 🔬 |
| P5 Foundation | `#2A0D0D → #B71C1C` | `#FFEBEE` | 🔴 |

---

## 📋 Banner Template (copy & paste, edit 4 fields)

```html
<div style="background:linear-gradient(135deg, [DARK] 0%, [MID] 100%);
     padding:36px 40px; border-radius:12px; margin-bottom:8px;">
  <div style="display:flex; align-items:center; gap:16px;">
    <span style="font-size:48px;">[EMOJI]</span>
    <div>
      <p style="color:#ADE8F4; margin:0; font-size:13px; letter-spacing:3px;
         text-transform:uppercase; font-family:monospace;">
        Computer Vision for Remote Sensing · Bangladesh
      </p>
      <h1 style="color:#FFFFFF; margin:4px 0 0 0; font-size:28px; font-family:monospace;">
        Phase [N] · [PHASE TITLE]
      </h1>
    </div>
  </div>
  <hr style="border-color:#1E88E5; margin:20px 0 16px 0;"/>
  <div style="display:flex; gap:32px; flex-wrap:wrap;">
    <span style="color:#90CAF9; font-family:monospace; font-size:13px;">
      📘 Lesson <b style='color:#FFF'>L[N] / [TOTAL]</b></span>
    <span style="color:#90CAF9; font-family:monospace; font-size:13px;">
      ⏱ Est. Time <b style='color:#FFF'>[X] hrs</b></span>
    <span style="color:#90CAF9; font-family:monospace; font-size:13px;">
      🔴 Priority <b style='color:#FFF'>Critical</b></span>
    <span style="color:#90CAF9; font-family:monospace; font-size:13px;">
      📍 Study Area <b style='color:#FFF'>[YOUR AREA]</b></span>
    <span style="color:#90CAF9; font-family:monospace; font-size:13px;">
      📅 Date <b style='color:#FFF'>____-__-__</b></span>
  </div>
</div>
```

---

## 📋 Exercise Box Template

```html
<div style="background:#FFF9C4; border-left:4px solid #F9A825;
     padding:14px 20px; border-radius:0 8px 8px 0;">
  <b>🏋️ Your Turn:</b> [TASK DESCRIPTION]<br/>
  Questions to answer:
  <ul style="margin:8px 0 0 0;">
    <li>[Question 1]</li>
    <li>[Question 2]</li>
  </ul>
</div>
```

---

## 📋 Takeaways Footer Template

```html
<div style="background:linear-gradient(135deg, [DARK] 0%, [MID] 100%);
     padding:24px 32px; border-radius:10px;">
  <h2 style="color:#FFFFFF; margin:0 0 12px 0; font-size:18px;">
    ✅ Key Takeaways — L[N]
  </h2>
  <ul style="color:#C8E6C9; font-size:14px; line-height:2.2; margin:0;">
    <li>[Takeaway 1]</li>
    <li>[Takeaway 2]</li>
    <li>[Takeaway 3]</li>
  </ul>
</div>

---
<div style="display:flex; justify-content:space-between; padding:10px 0;
     font-size:13px; color:#9E9E9E;">
  <span>← Previous: <a href='L[N-1]_[name].ipynb'>L[N-1]</a></span>
  <b style="color:#1565C0;">Phase [P] · L[N] of [TOTAL]</b>
  <span><a href='L[N+1]_[name].ipynb'>Next: L[N+1] →</a></span>
</div>
```

---

## 📁 Naming Convention

```
notebooks/
  phase1_raster_foundations/
    L1_image_as_tensor.ipynb
    L2_spatial_profile.ipynb
    L3_spectral_indices.ipynb
    L4_reprojection_resampling.ipynb
    L5_patch_tiling.ipynb
    L6_normalization.ipynb
    L7_visualization_qc.ipynb
  phase2_classical_ml/
    L1_feature_stack.ipynb
    L2_training_from_shapefiles.ipynb
    ...
```

**Rules:**
- Always `L[number]_[snake_case_title].ipynb`
- One concept per notebook — never combine L1+L2
- Fill in the `Date` field in the banner when you complete it
- Always run "Restart & Run All" before committing

---

## 🔄 Git Workflow — Push Every Lesson

```bash
# After completing each lesson:
cd cv-geospatial-roadmap

git add notebooks/phase1_raster_foundations/L1_image_as_tensor.ipynb
git add outputs/figures/phase1/L1_bands.png

git commit -m "✅ P1-L1: Image as tensor — Sitakunda S2 explored"

git push origin main
```

### Commit Message Convention

```
✅ P[phase]-L[lesson]: [short description]

Examples:
  ✅ P1-L3: Spectral indices — MNDWI flood mask Bhairab
  ✅ P2-L3: RF LULC — 5 classes, OA=87.3% Chittagong EPZ
  ✅ P3-L5: U-Net trained — flood IoU=0.74 Sen1Floods11
  🔧 P1-L5: Fix nodata threshold patch tiling
  📝 P4D-L4: Notes on yield regression BBS data
```

---

## ✅ Pre-Push Checklist (Every Notebook)

Before `git push`, make sure:

- [ ] Kernel → Restart & Run All — no errors
- [ ] Date filled in the banner
- [ ] Exercise cell has your answer (not blank)
- [ ] Notes table filled in
- [ ] Figure saved to `outputs/figures/`
- [ ] No absolute paths (use `pathlib.Path("../../data/...")`)
- [ ] No API keys or credentials in any cell
