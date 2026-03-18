# DataVault — Dataset Catalog

A self-contained, browser-based dataset catalog that lets teams discover, filter, and request access to curated AI/ML training datasets across image, video, audio, and document modalities.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset Library](#dataset-library)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage Guide](#usage-guide)
- [Contact & Licensing](#contact--licensing)

---

## Overview

DataVault is a single-file HTML application that serves as an internal or client-facing data catalog. It provides a rich, interactive UI for browsing 52+ curated datasets spanning computer vision, NLP, speech, biometrics, surveillance, and more. No backend or build step is required — just open the HTML file in a browser.

---

## Features

- **Full-text search** across dataset names, descriptions, and tags
- **Multi-attribute filtering** by modality, region, domain, file type, language, and license
- **Custom filter creation** — define and save your own filter dimensions on the fly
- **Drag-to-reorder** filter sidebar for personalised layouts
- **Sort options** — by relevance, name (A→Z), data volume, or newest
- **Dataset detail panel** with executive summary, specifications table, sample previews, and use-case breakdowns
- **Contact / inquiry form** embedded per dataset for licensing and pricing queries
- **Zero dependencies** — pure HTML + CSS + vanilla JavaScript, runs offline

---

## Dataset Library

The catalog currently contains **52 datasets** across four modalities:

### 🖼️ Image (19 datasets)
| ID | Title |
|----|-------|
| DS-001 | Urban Japanese & Korean Text Detection Image Dataset |
| DS-006 | Pet Image Collection |
| DS-007 | US Store Image Collection |
| DS-008 | Japan Stations Collection |
| DS-009 | Curated Image Dataset Collection |
| DS-010 | BP — Retail Store & Station |
| DS-012 | US Kitech Image Collection |
| DS-015 | Off-the-Shelf Image Datasets |
| DS-016 | Image Sets Structure |
| DS-017 | People Wearing Masks (Multi-Ethnicity) |
| DS-018 | Age Progression Images |
| DS-022 | Selfie Image Collection |
| DS-030 | Face Attribute Recognition Dataset |
| DS-036 | Extreme Density Crowd Counting Dataset |
| DS-037 | Large-Scale Dense Crowd Counting & Localization Dataset |
| DS-045 | Urban Geo-Localization Street View Image Dataset |
| DS-051 | Fine-Grained Dog Breed Image Classification Dataset |
| DS-052 | Visual-Semantic Image Captioning & Region Alignment Dataset |
| DS-053 | Digital Art PSD Collection |

### 🎬 Video (20 datasets)
| ID | Title |
|----|-------|
| DS-002 | Multiregional Face Analysis Video Dataset |
| DS-013 | Avatar Video Recording |
| DS-014 | Lip Sync and Video Recording |
| DS-021 | In-Car Video Collection |
| DS-029 | Athletic Action Video Recognition Dataset |
| DS-031 | Comprehensive YouTube Action Recognition Dataset |
| DS-032 | Web Video Action Classification Dataset |
| DS-033 | Aerial Surveillance Action Recognition Dataset |
| DS-034 | Multi-Viewpoint Human Action Dataset |
| DS-038 | Dynamic Crowd Flow Segmentation Dataset |
| DS-039 | Wide-Area Aerial Surveillance Tracking Dataset |
| DS-040 | High-Density Crowd Tracking & Floor Field Dataset |
| DS-041 | Multi-Person Parking Lot Tracking Dataset |
| DS-042 | Video-Based Fire & Flame Detection Dataset |
| DS-043 | Large-Scale Aerial Surveillance Event Recognition Dataset |
| DS-044 | Comprehensive Visual Object Tracking Benchmark |
| DS-046 | Real-World 50-Category YouTube Action Recognition Dataset |
| DS-047 | Moving Camera Action Recognition via Lagrangian Motion Decomposition |
| DS-048 | Multimodal Surveillance Video-Language Understanding Dataset |
| DS-049 | Real-World YouTube Action Video Dataset with XML Annotations |

### 🔊 Audio (3 datasets)
| ID | Title |
|----|-------|
| DS-003 | Audio Sourcing |
| DS-005 | Cross-Industry Audio Recordings |
| DS-019 | Indonesia Audio Samples |

### 📄 Document (10 datasets)
| ID | Title |
|----|-------|
| DS-004 | Real-World Hindi Financial & Legal Documents Dataset |
| DS-020 | Japanese Document Collection |
| DS-023 | Enterprise Financial Analysis Prompt Benchmark |
| DS-024 | Cultural German Evaluation Dataset |
| DS-025 | GenAI FTE Evaluation Dataset |
| DS-026 | News Prompts Classification Dataset |
| DS-027 | WhatsApp Summarization Dataset |
| DS-028 | Reels Coherence QA Dataset |
| DS-035 | Smartphone Inertial Motion Activity Dataset |
| DS-050 | Parameterized Human Motion Capture Dataset |

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

The entire application — HTML structure, CSS styles, dataset definitions, and JavaScript logic — lives in the single HTML file. Dataset records (`DS-001` through `DS-053`) are defined as a JavaScript array (`const DS`) embedded in the file.

---

## Usage Guide

### Searching
Type any keyword into the **search bar** at the top. Results are filtered in real time across dataset titles, descriptions, domains, and tags.

### Filtering
Use the **filter sidebar** on the left to narrow results by:
- **Modality** — Image, Video, Audio, Document
- **Region** — Asia, US, Europe, Global, etc.
- **Domain** — OCR/Text, Biometric, Speech/NLP, Computer Vision, Retail, Automotive, etc.
- **File Type** — JPEG, PNG, MP4, WAV, PDF, etc.
- **Language** — Japanese, Korean, Hindi, German, Indonesian, etc.
- **License** — Commercial, Research, etc.

Filters can be **dragged to reorder** and **collapsed** to save space.

### Custom Filters
Click **"Create Custom Filter"** to define your own filter dimension with a name and comma-separated values.

### Sorting
Use the **Sort** dropdown to order results by Relevance, Name (A→Z), Volume (High→Low), or Newest First.

### Dataset Details
Click any dataset card to open a detailed panel containing:
- Executive summary
- Full specification table (format, size, annotation type, licensing, etc.)
- Sample images / previews
- Characteristic highlights
- Application use-cases

### Requesting a Dataset
Inside any dataset detail panel, click **"📂 View Full Dataset →"** to access the data link, or use the **"Contact Us"** overlay to send a licensing or pricing inquiry.

---

## Contact & Licensing

Dataset licensing varies per entry (Commercial or Research). To inquire about a specific dataset, use the **Contact Us** form embedded in each dataset's detail view. Inquiries are typically responded to within 24 hours.
