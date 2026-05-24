# 🛰️ Computer Vision for Remote Sensing & Agriculture
### A Self-Paced Learning Roadmap — Bangladesh Focus

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red?logo=pytorch)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

---

## 📌 About This Repository

This repository documents my learning journey in **Geospatial Computer Vision**, covering
satellite image analysis, deep learning for remote sensing, UAV/drone imagery, agricultural
CV, and population estimation — applied to **Bangladesh study areas** (Sitakunda, Chittagong
EPZ, Sundarbans, Dhaka, Sylhet Haor).

Built alongside a structured 19-week roadmap using Sentinel-1/2, Landsat, GEDI, UAV imagery,
and LiDAR data.

---

## 🗂️ Repository Structure

```
cv-geospatial-roadmap/
│
├── 📓 notebooks/
│   ├── phase1_raster_foundations/     ← Raster basics, band math, tiling
│   ├── phase2_classical_ml/           ← Random Forest, SVM, OBIA
│   ├── phase3_deep_learning/          ← PyTorch, U-Net, transfer learning
│   ├── phase4_geo_dl/                 ← TorchGeo, GEDI, LiDAR
│   ├── phase4d_agri_satellite/        ← Crop mapping, yield prediction
│   ├── phase4e_uav/                   ← UAV processing, YOLOv8, disease
│   ├── phase4f_disease/               ← PlantVillage, Grad-CAM, phenology
│   └── phase5_foundation_models/      ← NASA Prithvi, SAM, SatMAE
│
├── 🧰 src/
│   ├── raster_utils.py                ← Shared rasterio helpers
│   ├── indices.py                     ← Spectral index functions
│   ├── patching.py                    ← Tiling and patch management
│   ├── visualization.py               ← Reusable plot functions
│   └── normalize.py                   ← Dataset normalization
│
├── 📊 outputs/
│   └── figures/                       ← Saved plots and maps
│
├── 📁 data/
│   └── sample/                        ← Small sample data for testing
│   (raw/, patches/, stats/ are gitignored — too large)
│
├── environment.yml                    ← Conda environment
├── requirements.txt                   ← pip install list
└── .gitignore
```

---

## 🗺️ Roadmap Progress

| Phase | Title | Status | Notebooks |
|-------|-------|--------|-----------|
| P1 | Raster CV Foundations | 🟡 In Progress | 7 lessons |
| P2 | Classical ML Baseline | ⬜ Planned | 7 lessons |
| P3 | Deep Learning Core | ⬜ Planned | 9 lessons |
| P4A | Semantic Segmentation | ⬜ Planned | 5 lessons |
| P4B | Canopy Height Regression | ⬜ Planned | 5 lessons |
| P4C | LiDAR Point Cloud | ⬜ Planned | 6 lessons |
| P4D | Agri CV — Satellite | ⬜ Planned | 6 lessons |
| P4E | UAV Agri CV | ⬜ Planned | 8 lessons |
| P4F | Crop Disease & Growth | ⬜ Planned | 7 lessons |
| P5  | Foundation Models | ⬜ Planned | 6 lessons |

---

## 🌍 Study Areas

| Area | Country | Data Used | Phase |
|------|---------|-----------|-------|
| Sitakunda | Bangladesh | Sentinel-2, Landsat | P1–P4A |
| Chittagong EPZ | Bangladesh | Sentinel-2, Landsat | P2, P4A |
| Bhairab | Bangladesh | Sentinel-1 SAR | P2–P4A |
| Sundarbans | Bangladesh | GEDI, Sentinel-2 | P4B |
| Sylhet Haor | Bangladesh | Sentinel-2 time series | P4D |
| Dhaka | Bangladesh | Landsat TIR, LiDAR | P4C |

---

## ⚙️ Setup

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/cv-geospatial-roadmap.git
cd cv-geospatial-roadmap

# Create conda environment
conda env create -f environment.yml
conda activate gis_ml

# Or with pip
pip install -r requirements.txt

# Launch VS Code with Jupyter
code .
```

---

## 📦 Key Libraries

`rasterio` · `geopandas` · `PyTorch` · `torchgeo` · `segmentation-models-pytorch`
`albumentations` · `ultralytics` · `cropharvest` · `timm` · `open3d` · `laspy`

---

## 📬 Contact

**Study Area:** Bangladesh | **Focus:** Geospatial CV, Remote Sensing, Precision Agriculture
