# ESG Performance Dashboard — Retail Operations


## Overview
This project analyzes Environmental, Social, and Governance (ESG) performance across 50 retail store locations using three datasets covering governance, environmental, and social workforce metrics (60,000+ records total). The goal was to surface operational patterns that aggregate ESG scores tend to hide.

## Business Problem
Retail organizations report ESG scores as single headline numbers but those numbers can mask significant variation across regions, store locations, and time periods. This dashboard was built to answer: where are the real risks, and what's actually driving them?

## Dashboard Pages
- **Overview** — Overall ESG score (75.01), component scores (E/S/G), regional performance, and store-level risk classification
<img width="878" height="539" alt="e20" src="https://github.com/user-attachments/assets/2d3a7d62-d3f8-4fe6-b596-321ea54e2361" />

- **Environmental** — Carbon emissions trends, energy consumption, recycling rate (58.04%), waste by category, and store-level compliance breakdown
<img width="875" height="528" alt="E22" src="https://github.com/user-attachments/assets/8ef240c7-c7db-4d1c-881e-fc5d831e54dd" />
  
- **Social** — Workforce composition (3.22M employees), turnover rate (22.48%), satisfaction scores, safety incidents, and diversity metrics by region
<img width="877" height="537" alt="E21" src="https://github.com/user-attachments/assets/9b6a8886-7ef1-441a-b62b-771485cdf820" />

- **Governance** — Compliance rate (70.14%), GDPR adherence (84.99%), regulatory penalties ($998.41M), ethics violations, and cybersecurity investment vs data breach incidents
<img width="888" height="534" alt="E23" src="https://github.com/user-attachments/assets/7a808a39-02b4-4aa8-a0de-54af35ec998c" />

## Key Findings
- Carbon emissions spike consistently in August–September across all regions, correlating directly with peak energy consumption a pattern that points to seasonal operational decisions rather than infrastructure
- Packaging waste accounts for 40% of all waste generated (20.38M kg), making it the highest-impact target for waste reduction programmes
- Employee turnover at 22.48% is high despite satisfaction scores being consistent at 4.0/5 across all regions — satisfaction alone is not predicting retention
- Total regulatory penalties of $998.41M sit against a 70.14% compliance rate, suggesting that partial and non-compliant stores carry disproportionately high penalty exposure
- High-risk stores cluster below the 75 ESG score threshold in the scatter analysis, creating a clear segmentation line for intervention

## Tools & Techniques
- **Power BI** — 4-page interactive dashboard with cross-filtering across all visuals
- **DAX** — Custom measures including weighted recycling rate (`DIVIDE(SUM recycled, SUM generated)`), compliance rate, ESG component scores, and risk classification logic
- **Data modelling** — Relationships built across 3 separate datasets joined on Store_Location and Date
- **Datasets** — ESG_Governance_Corporate_Metrics.csv, ESG_Environmental_Waste_Metrics.csv, ESG_Social_Workforce_Metrics.csv

## Files in This Repository
| File | Description |
|---|---|
| ESG_Governance_Corporate_Metrics.csv | Governance and compliance dataset |
| ESG_Environmental_Waste_Metrics.csv | Environmental and waste metrics dataset |
| ESG_Social_Workforce_Metrics.csv | Social and workforce metrics dataset |
| overview.png | Overview dashboard screenshot |
| environmental.png | Environmental dashboard screenshot |
| social.png | Social dashboard screenshot |
| governance.png | Governance dashboard screenshot |

---
*Designed by Jacqline | Power BI | Data Analytics*
