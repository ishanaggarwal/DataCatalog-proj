# DataVault — Dataset Catalog

A self-contained, browser-based dataset catalog that lets teams discover, filter, and request access to curated AI/ML training datasets across image, video, audio, and document modalities.

> **Latest update (2026-04-02):** The catalog now includes new datasets (DS-054 through DS-056) and adds a **dark/light theme toggle**, a **sample preview modal** (with full-screen image viewer), and a **Preprocessing Tools** dropdown in the sidebar.

---

## Table of Contents

- [Overview](#overview)
- [What’s New](#whats-new)
- [Features](#features)
- [Dataset Library](#dataset-library)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage Guide](#usage-guide)
- [Contact & Licensing](#contact--licensing)

---

## Overview

DataVault is a single-file HTML application that serves as an internal or client-facing data catalog. It provides a rich, interactive UI for browsing curated datasets spanning computer vision, NLP, speech, biometrics, surveillance, and more. No backend or build step is required — just open the HTML file in a browser.

---

## What’s New

Changes reflected in `datavault-client_iteration18 (1).html`:

- **New datasets** added to the library: **DS-054**, **DS-055**, **DS-056**.
- **Dark/Light mode** toggle (persists via `localStorage`).
- **Preview Sample modal** for datasets with sample media:
  - Image grid preview
  - **Fullscreen viewer** for zooming images
  - For sample entries with a `link`, clicking opens the source (e.g., Drive / hosted link)
- **Preprocessing Tools** dropdown in the sidebar (external tools shortcuts).
- **Active filter chips bar** to view/remove active filters quickly.

---

## Features

- **Full-text search** across dataset names, descriptions, and tags (with synonym expansion)
- **Multi-attribute filtering** by modality, region, domain, file type, language, and annotation
- **Custom filter creation** — define and save your own filter dimensions on the fly
- **Drag-to-reorder** filter sidebar for personalised layouts + collapse sections
- **Sort options** — by relevance, name (A→Z), data volume, or newest
- **Pagination controls** with page-size selector (including an “All” option)
- **Dataset detail panel** with executive summary, specifications table, and use-case breakdowns
- **Preview samples** (modal + fullscreen image viewer) for datasets that include sample media
- **Contact / inquiry form** embedded per dataset for licensing and pricing queries
- **Zero dependencies** — pure HTML + CSS + vanilla JavaScript, runs offline

---

## Dataset Library

The catalog currently contains **56 datasets** across four modalities:

### 🖼️ Image
(See catalog UI for the full, up-to-date listing.)

### 🎬 Video
(See catalog UI for the full, up-to-date listing.)

### 🔊 Audio
(See catalog UI for the full, up-to-date listing.)

### 📄 Document
Includes newly added:
- **DS-054 — Document Collection (HR + Medical)**
- **DS-055 — Tokyo POI Data Collection Pilot**
- **DS-056 — Lucknow POI Collection Dataset**

---

## Getting Started

No installation, build step, or internet connection is required.

1. **Clone the repository**
   ```bash
   git clone https://github.com/ishanaggarwal/DataCatalog-proj.git
   cd DataCatalog-proj
   ```

2. **Open the catalog in your browser**
   ```bash
   # macOS
   open "datavault-client_iteration18 (1).html"

   # Linux
   xdg-open "datavault-client_iteration18 (1).html"

   # Windows
   start "datavault-client_iteration18 (1).html"
   ```
   Or simply double-click the file in your file manager.

---

## Project Structure

```
DataCatalog-proj/
├── datavault-client_iteration18 (1).html   # Main catalog application (self-contained)
└── README.md                               # This file
```

The entire application — HTML structure, CSS styles, dataset definitions, and JavaScript logic — lives in the single HTML file.

---

## Usage Guide

### Searching
Type any keyword into the **search bar** at the top. Results are filtered in real time across dataset titles, descriptions, and tags.

### Filtering
Use the **filter sidebar** on the left to narrow results by:
- **Modality** — Image, Video, Audio, Document
- **Annotation** — (where available)
- **Region** — Asia, US, Europe, Global, etc.
- **Domain** — OCR/Text, Biometric, Speech/NLP, Computer Vision, Retail, Automotive, etc.
- **File Type** — JPEG, PNG, MP4, WAV, PDF, etc.
- **Language** — Japanese, Korean, Hindi, German, Indonesian, etc.

Filters can be **dragged to reorder** and **collapsed** to save space. Active filters appear as **chips** above the grid and can be removed individually.

### Custom Filters
Click **"Create Custom Filter"** to define your own filter dimension with a name and comma-separated values.

### Sorting + Page Size
Use the **Sort** dropdown to order results by Relevance, Name (A→Z), Volume (High→Low), or Newest First.
Use the **page-size** selector to control how many tiles show per page (or choose **All**).

### Preview Samples
For datasets that include sample media, click **Preview Sample** to open a modal with sample images/clips/files. For zoomable samples, click to open the fullscreen viewer (or open external links when provided).

### Requesting a Dataset
Inside any dataset detail panel, click **"📂 View Full Dataset →"** to access the data link (when available), or use the **"Contact Us"** overlay to send a licensing or pricing inquiry.

---

## Contact & Licensing

Dataset licensing varies per entry (Commercial or Research). To inquire about a specific dataset, use the **Contact Us** form embedded in each dataset's detail view.