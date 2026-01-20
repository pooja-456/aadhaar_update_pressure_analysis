# Aadhaar Update Pressure Analysis

A district-level, data-driven analysis of Aadhaar enrolment and demographic update patterns to identify update pressure, lifecycle maturity, and regional inefficiencies for targeted UIDAI administrative action.

---

## Project Context
This project was developed as part of the **Online Hackathon on Data-Driven Innovation for Aadhaar**, organised by **UIDAI in association with NIC and MeitY**.

---

## Problem Statement
Although Aadhaar has achieved near-universal enrolment, several regions continue to experience disproportionately high demographic update activity. Raw enrolment or update counts alone fail to reveal operational imbalance, structural inefficiencies, or lifecycle maturity.

**Objective:**  
Analyse anonymised Aadhaar enrolment and update data to uncover temporal, geographic, and demographic patterns that indicate persistent update pressure and administrative inefficiencies at the district level.

---

## Analytical Framework
The analysis follows a structured, lifecycle-aware EDA approach across four layers:

- **WHEN** – Monthly enrolment vs update trends  
- **WHERE** – State and district-level concentration  
- **WHO** – Age-group driven enrolments and updates  
- **WHY** – Update-to-enrolment ratios to detect inefficiencies  

---

## Key Metric
**Update-to-Enrolment Ratio**

This metric normalises demographic update volume by enrolment activity to:
- Capture Aadhaar lifecycle maturity
- Identify update-dominant districts
- Detect structural operational stress

Safeguards include minimum thresholds to avoid low-denominator distortion.

---

## Datasets Used
- Aadhaar Enrolment Dataset (aggregated counts by age group)
- Aadhaar Demographic Update Dataset (aggregated update activity)

**Data Compliance**
- Fully anonymised and aggregated
- No personal identifiers
- No external datasets
- Missing months retained without imputation

---

## Methodology
- Multi-file CSV ingestion using Python (pandas)
- Standardisation of state and district names
- District-level aggregation using:
  `groupby(["state_final", "district_norm"])`
- Monthly aggregation for temporal analysis
- Validation through shape and total preservation checks

---

## Key Insights
- Aadhaar operations are increasingly **update-driven**
- Update pressure is **systemic**, not isolated
- Adult demographic updates dominate system load
- Several non-metro districts exhibit persistent high update pressure

---

## Tools & Technologies
- Python
- pandas, numpy
- matplotlib
- Jupyter Notebook (VS Code)

---

## Reproducibility
All steps from ingestion to EDA are implemented in Jupyter notebooks.  
Run the notebooks sequentially to reproduce the analysis.

---

## Impact
The analysis demonstrates that Aadhaar has transitioned from an enrolment-centric system to an update-dominated lifecycle system, highlighting the need for district-level, data-driven administrative planning by UIDAI.
