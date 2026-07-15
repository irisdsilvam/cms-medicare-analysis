# CMS Medicare Part D — Spending Anomaly Analysis

Independent analysis of CMS public Medicare Part D prescriber data 
to identify spending anomalies and provider-level trends in support 
of program oversight objectives.

## Key Findings

### Spending Anomaly Analysis
- **Sample analyzed:** 500,000 records from CMS Medicare Part D 2024 dataset
- **Unique prescribers:** ~21,000
- **Average spending per prescriber:** $196,535
- **Anomaly threshold (mean + 2σ):** $1,543,884
- **Anomalous prescribers identified:** 510 (2.4% of total)
- **Top outlier:** Family Practice prescriber with $41.7M in drug costs — 
  27x above the anomaly threshold

### Geographic Risk Analysis
- **Highest anomaly rate state:** Alabama (5.1% of prescribers flagged)
- **States above national average:** 15 of 50 states analyzed
- **Regional pattern:** Southern and Midwest states show disproportionate 
  concentration of anomalous prescribers
- **Key insight:** Rate-based and per-1,000-prescriber normalization corrects 
  for population size bias, surfacing smaller states with elevated risk

## Methodology
- Statistical anomaly detection using mean + 2 standard deviations
- Spending aggregated by prescriber NPI across all drug categories
- State-level analysis normalized by total prescriber population per state
- Visualizations highlight distribution skew, high-cost outliers, and geographic patterns

## Tools
Python · pandas · matplotlib · Jupyter Notebooks · Git · CMS Open Data

## Privacy Note
All prescriber identities are anonymized. Analysis uses aggregate 
spending patterns only.
