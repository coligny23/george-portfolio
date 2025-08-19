---
layout: page
title: Anchor C — Pilot A/B Design: SMS Nudge for Food-Waste Reduction
permalink: /anchors/anchor-c/
---

## Overview
A **pre-analysis plan (PAP)** for a small randomized pilot that tests whether periodic SMS reminders/market info increase recovery and redistribution of surplus produce.

## Objectives & Hypotheses
- **H1 (ITT):** Households/collectors receiving SMS nudges show higher **kg of surplus produce recovered per week** versus control.  
- **H2:** Treated units report **more transactions** (count) and **higher app engagement** (if applicable).  
- **H3 (exploratory):** Price dispersion narrows in treated areas during surplus periods.

## Intervention & Unit
- **Intervention:** 1–2 SMS/week with actionable tips (where/when to sell/donate; storage/transport tips).  
- **Unit of randomization:** Household or community group (specify).  
- **Duration:** 6–8 weeks.

## Outcomes & Measurement
- **Primary:** kg of recovered produce/week (self-report with periodic verification).  
- **Secondary:** number of transactions; app open rate/click-through; revenue from surplus.  
- **Covariates:** baseline access (from **Anchor B**), household size, typical harvest window.

## Design & Randomization
- **Arms:** Treatment (SMS) vs. Control (no SMS).  
- **Stratification:** by ward/access tercile to improve balance.  
- **Assignment:** reproducible seed, documented in code.

## Sample Size & Power (illustrative)
- Minimum detectable effect set to **Δ = 0.25–0.40 SD** of baseline recovery.  
- Power = 0.80, α = 0.05; intra-cluster correlation assumed ρ = 0.05 (if clustered).  
- Simulations in `/notebooks/07_power_calc.ipynb` produce power curves by N and Δ.

## Analysis Plan
- **Primary:** ITT difference in means and OLS with pre-specified covariates.  
- **SEs:** robust/clustered as appropriate.  
- **Heterogeneity (exploratory):** by access tercile (from Anchor B) and season.  
- **Multiple outcomes:** control FDR or present a sharpened q-value panel.

## Ethics, Privacy & Risks
- Informed consent; opt-out in every SMS.  
- Minimal PII, hashed IDs, secure storage; comply with local regulations.  
- Risks: message fatigue, misinformation; mitigations: frequency caps, vetted templates.

## Timeline (example)
- **Week 0:** Baseline, randomization, consent.  
- **Weeks 1–6:** Intervention & monitoring.  
- **Week 7–8:** Endline, analysis, brief.

## Artifacts
- Design doc (PDF): `/reports/anchor_c_design.pdf`  
- Pre-analysis plan (Markdown/PDF): `/reports/anchor_c_pap.pdf`  
- Power simulation: `/notebooks/07_power_calc.ipynb`  
- *(Optional)* Registration (OSF/AEA): **[Add link when registered]**

## Next Steps
- Pilot message content with 5–10 users; refine tone and timing.  
- If effects are promising, scale with stratified rollout and cost-effectiveness analysis.  
- Combine with logistics partnerships identified in **Anchor B** hotspots.

## Reproducibility
- All simulated analyses are scripted and seeded.  
- Final code, PAP, and de-identified aggregates will be published.  
- See **`/ethics`** page and `DATA_SOURCES.md` for governance and licensing.

> **Licensing:** Text & design © George Odongo — **CC BY 4.0**. Code under **MIT/Apache-2.0**.
