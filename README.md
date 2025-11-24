# MUSA 5500 Final Project  
## Bus Transport Accessibility Analysis Across Global Cities

## 🔗 Website

Interactive project website (hosted on GitHub Pages):  
https://zonghuali77-rgb.github.io/MUSA-5500-Final-Project/

GitHub repository:  
https://github.com/zonghuali77-rgb/MUSA-5500-Final-Project

---

## 📘 Project Overview

This project analyzes **public bus accessibility** in four global cities (New York, Singapore, Amsterdam, and Shanghai) using spatial analytics.  
The objectives are to:

- Quantify the spatial distribution of bus stops and service coverage.
- Compare accessibility patterns across different urban forms and planning regimes.
- Identify areas of potential under-provision of bus services within each city.

The analysis is exploratory and methodologically focused rather than demand-based (no ridership data), emphasizing how far publicly available spatial data can support comparative transit accessibility research.

---

## 📂 Repository Contents

This GitHub repository contains **all materials required for the course submission**, including:

- HTML files for the deployed GitHub Pages website.
- Quarto-generated pages for each case-study city and the methods/results sections.
- Jupyter notebook used for data wrangling, spatial analysis, and figure export.
- Raw and processed GIS datasets (boundaries, bus stops, intermediate layers).
- Static figures and image assets used in the website.
- Supporting files created automatically by Quarto (`site_libs`, search index, etc.).

---

## 📊 Methods Summary

A concise outline of the analytical workflow:

1. **Data acquisition**
   - City administrative boundaries from open government portals and curated GIS sources.
   - Bus stop locations from OpenStreetMap and official open data portals (e.g., LTA, NYC Open Data).
   - Reference bus-line maps for qualitative comparison of network structure.

2. **Spatial preprocessing**
   - Reprojection to appropriate projected coordinate systems for each city.
   - Clipping bus stops to harmonized “analysis extents” focused on the continuous urbanized area.
   - Handling inconsistencies between administrative boundaries and built-up areas.

3. **Accessibility and network metrics**
   - Bus stop **point density** (KDE) at multiple spatial scales.
   - **Nearest-neighbour distance** statistics for stops within each city.
   - Coverage analysis using buffer distances to approximate walk-sheds.
   - Simple city-level indicators (e.g., stops per km² of built-up area) for cross-city comparison.

4. **Visualization and communication**
   - Export of maps and indicators to static figures.
   - Assembly of an interactive, multi-page website using Quarto, combining text, figures, and web-ready graphics.

---

## 📁 File Structure

Key folders and files in this repository:

- `data/`  
  Raw and processed spatial data, including city boundaries, bus stop point layers, and intermediate GIS outputs (e.g., GeoJSON, shapefiles).

- `figures/`  
  Exported analytical figures (maps, charts) used in the final website and report.

- `image/`  
  Additional images such as reference bus-line maps and layout graphics.

- `site_libs/`  
  Libraries and support files generated automatically by Quarto for the website (do not edit manually).

- `website/`  
  Quarto source pages (`.qmd` / converted `.html`) for city-specific sections and project sub-pages.

- `Transportation Accessibility Project.html`  
  Main compiled HTML document containing the full stitched site as exported from Quarto.

- `index.html`  
  Entry point for the GitHub Pages site (redirects or links into the main project content).

- `search.json`  
  Auto-generated search index for the website.

- `Transportation Accessibility Project-checkpoint.ipynb` (or similar notebook file)  
  Jupyter notebook with the analysis pipeline: data loading, spatial joins, metric calculation, and figure export.

- `README.md`  
  The document you are currently reading, summarizing the project and repository structure.

---

## 👩‍💻 Author

**Zonghua Li**  
Master of City Planning (MCP)  
University of Pennsylvania — MUSA 5500  
Fall 2025
