---
layout: page
title: Anchor A — Food Insecurity Snapshot (Tanzania)
permalink: /anchors/anchor-a/
---

## Overview
A concise, reproducible look at recent food security indicators relevant to SDG 2 (Zero Hunger), with simple trends and uncertainty where possible. The goal is clarity over complexity and a policy-friendly summary.

## Question
What do recent, publicly available indicators suggest about food insecurity in Tanzania, and what short insights are actionable for practitioners?

## Context & SDGs
- **Primary SDG:** 2 (Zero Hunger)  
- **Related:** 12 (Responsible Consumption & Production), 13 (Climate Action)

## Data Sources (open)
- **World Bank / World Development Indicators** (e.g., prevalence of undernourishment, CPI food, poverty headcount).  
- **FAOSTAT** (food balances, supply/utilization, commodity groups).  
- *(Optional, if used)* **WFP mVAM** or national survey extracts.  
- See **`/DATA_SOURCES.md`** for exact tables, URLs, and licenses (e.g., World Bank & FAOSTAT: CC BY 4.0).

> **Note:** Raw/large data are not committed. This page links to processed outputs and code.

## Methods (brief)
- Load & clean series with **pandas**.  
- Harmonize units, align years, handle missing data transparently.  
- Produce **3 core charts** (e.g., undernourishment trend, per-capita supply proxy, food CPI).  
- Add simple uncertainty bands where metadata allows.  
- Document all steps in notebooks; keep figures lightweight for the web.

## Artifacts
- Notebook(s):  
  - `/notebooks/03_pandas_intro.ipynb`  
  - `/notebooks/04_clean_viz.ipynb`  
- Brief (≤ 600 words, PDF): `/reports/anchor_a_brief.pdf`  
- Figures:  
  - `/assets/anchor_a_fig1.png`  
  - `/assets/anchor_a_fig2.png`  
  - `/assets/anchor_a_fig3.png`  
- *(Optional)* Dashboard: **[Add public link here]**

## Key Findings (example placeholders)
1. *Indicator X* shows a **directional change** since year Y; confidence limited by data gaps in Z.  
2. Food price pressure (CPI-food) diverges from regional average since YYYY—implications for targeting.  
3. Proxy availability suggests seasonal sensitivity; monitoring cadence should be increased in months M–N.

## Limitations
- Mixed data vintages; series definitions differ by source.  
- Indicators are **proxies**, not direct measures of household food access.  
- National aggregates may mask sub-national heterogeneity.

## Next Steps
- Add sub-national cuts (if available) and robustness checks.  
- Integrate a simple affordability index (prices × incomes).  
- Link to geospatial access constraints (see **Anchor B**).

## Reproducibility
- Exact code and figure generation in the linked notebooks.  
- Environment & dependencies in `environment.yml`.  
- Data licensing and provenance in `DATA_SOURCES.md`.

> **Attribution:** Please cite original data providers. This page, text, and figures © George Odongo — released under **CC BY 4.0**. Code under **MIT/Apache-2.0** (see repo licenses).
