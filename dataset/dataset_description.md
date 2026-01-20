## Final Dataset Description

This folder contains cleaned, aggregated, and analysis-ready datasets
derived from official UIDAI Aadhaar enrolment and demographic update data.

These files are processed outputs used directly in the analysis notebooks.

### Files Overview

- **enrolment_aggregated.csv**  
  District-level aggregated Aadhaar enrolments by age group.

- **enrolment_monthly.csv**  
  Monthly enrolment data used for temporal trend analysis.

- **demographic_aggregated.csv**  
  District-level aggregated Aadhaar demographic update counts by age group.

- **demographic_monthly.csv**  
  Monthly demographic update data for temporal analysis.

- **persistent_high_pressure_districts.csv**  
  Districts exhibiting consistently high update-to-enrolment ratios
  after applying minimum threshold safeguards.

- **uidai_district_priority_table.csv**  
  Final district prioritisation table combining volume, ratios, and
  persistence to support UIDAI administrative decision-making.

### Data Note
Raw UIDAI datasets are not included in this repository.
Only processed, non-identifiable analytical outputs are stored here.
