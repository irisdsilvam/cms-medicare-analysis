# cms-medicare-analysis
Anomaly detection analysis on CMS Medicare Part D public dataset using Python
# CMS Medicare Part D — Spending Anomaly Analysis

Independent analysis of CMS public Medicare Part D prescriber data 
to identify spending anomalies and provider-level trends in support 
of program oversight objectives.

## Key Findings
- **Sample analyzed:** 500,000 records from CMS Medicare Part D 2024 dataset
- **Unique prescribers:** ~21,000
- **Average spending per prescriber:** $196,535
- **Anomaly threshold (mean + 2σ):** $1,543,884
- **Anomalous prescribers identified:** 510 (2.4% of total)
- **Top outlier:** Family Practice prescriber with $41.7M in drug costs — 
  27x above the anomaly threshold

## Methodology
- Statistical anomaly detection using mean + 2 standard deviations
- Spending aggregated by prescriber NPI across all drug categories
- Visualizations highlight distribution skew and high-cost outliers

## Privacy note
All prescriber identities are anonymized. 
Analysis uses aggregate spending patterns only.

## Tools
Python · pandas · matplotlib · Jupyter Notebooks · CMS Open Data
