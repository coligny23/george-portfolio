---
layout: page
title: Anchor B — Geospatial Barriers to Surplus-Produce Recovery
permalink: /anchors/anchor-b/
---

## Overview
A lightweight geospatial scan to highlight **physical access constraints** that hinder recovery and redistribution of edible but rejected produce—linking to SDG 2 & 12.

## Question
Where are clusters of smallholders/markets with **poor access** to aggregation or redistribution points, and what does that imply for low-cost interventions?

## Data Sources (open)
- **Tanzania admin boundaries** (e.g., GADM or national open portal).  
- **Roads/points of interest**: **OpenStreetMap** (markets, collection points; ODbL).  
- *(Optional)* **Population grids** (WorldPop/HRSL) for demand weighting.  
- See **`/DATA_SOURCES.md`** for URLs and licenses (OSM: ODbL).

## Methods (brief)
- Preprocess layers in **QGIS**.  
- Construct a simple **cost surface** using road class–based speeds (assumptions documented).  
- Compute **travel time/buffer** to nearest market/collection point.  
- Summarize at ward/district level (share > X minutes from nearest point).  
- Export web-friendly map and policy table.

## Artifacts
- Map (PNG/PDF):  
  - `/assets/anchor_b_map.png`  
  - `/assets/anchor_b_map.pdf`  
- Brief (≤ 800 words, PDF): `/reports/anchor_b_brief.pdf`  
- *(Optional)* QGIS project (small sample or style only): `/assets/qgis/anchor_b_project.qgz`  
- *(Optional)* Dashboard: **[Add public link here]**

## Key Findings (example placeholders)
1. Districts A, B show **>40%** of households beyond **60-minute** travel to markets on assumed speeds.  
2. A small number of **new aggregation points** (≤ N) on corridor C could reduce average travel time by **X%**.  
3. Seasonal road passability (rainy season) likely amplifies constraints; pilot planning should consider M–N months.

## Limitations
- Travel-time model uses **assumed speeds** and limited elevation/hydrology data.  
- OSM completeness varies by region; under-mapping possible.  
- Results indicate **relative** access, not guaranteed service availability.

## Next Steps
- Ground-truth a subset of hotspots with local partners.  
- Incorporate elevation/river crossings and seasonal effects.  
- Link to **Anchor C** to test messaging or logistics nudges in high-friction areas.

## Reproducibility
- Processing steps documented in a short how-to note: `/reports/anchor_b_methods.pdf`.  
- Styles and symbology saved within the QGIS project.  
- Source and license details in `DATA_SOURCES.md`.

> **Attribution:** OSM contributors (ODbL), other providers per their licenses. Text & figures © George Odongo — **CC BY 4.0**.
