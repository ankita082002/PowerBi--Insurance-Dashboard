# PowerBi--Insurance-Dashboard

# INSURANCE RISK & CLAIMS ANALYSIS

## Summary

Power BI dashboard analyzing **37,542** auto insurance policies and **\$187.8M** in claim amounts to understand risk and customer segments.

## Overview

An interactive Power BI report to monitor policy mix, claim behavior, and demographics. It surfaces KPIs, trends by vehicle and customer attributes, and a claims matrix by education and marital status.

## Problem Statement

Decision makers need a single view to:

* Track overall volume and claims
* See which segments (car use, make, zone, age, education) drive policies and claim amounts
* Compare claim amounts across marital and education groups

## Dataset

* **Type**: Auto insurance policies & claims (sample dataset)
* **Rows**: 37,542 policies
* **Key fields used**: `Gender`, `CarUse`, `CarMake`, `CoverageZone`, `AgeGroup`, `CarYear`, `KidsDriving`, `Education`, `MaritalStatus`, `ClaimAmount`, `ClaimFrequency`, `PolicyID`

## Tools and Technologies

* **Power BI Desktop**
* **DAX** for measures and calculated fields
* **Excel** as source file

## Methods

* Data cleaning (remove duplicates, standardize categories)
* **Measures**: Total Policies, Total Claim Amount, Average Claim Frequency, Average Claim Amount
* Visuals:

  * Donuts/Bars: Policies by **Car Use**, **Car Make**, **Coverage Zone**
  * Column chart: Policies by **Age Group**
  * Line chart: Policies by **Car Year** (1990–2020)
  * Histogram: Policies by **Kids Driving**
  * Pie: Policies by **Education**
  * Matrix: **Claim Amount by Education × Marital Status**
* Slicer: **Select measures** (e.g., Total Policies, Total Claim Amount)

## Key Insights

* **KPIs**: 37,542 policies • **\$187.8M** total claim amount • Avg claim freq **0.5** • Avg claim amount **\$5.0K**
* **Gender split**: Male **18.7K**, Female **18.8K** (balanced).
* **Car use**: Predominantly **Private (\~30K)** vs **Commercial (\~7K)**.
* **Top car makes by policies**: **Ford (\~3.3K)**, **Chevrolet (\~3.0K)**, then **Dodge/Toyota/GMC (\~1.8K)**.
* **Coverage zone**: Segments around \~20% each (Urban, Rural, Highly Urban, Suburban, Highly Rural).
* **Age groups**: Peaks around **36–65 (\~7.0–7.1K)**; lowest **15–25 (\~4.2K)**, **66–75 (\~5.1K)**.
* **Car year trend**: Growth through 2000s with peaks in early–mid 2010s.
* **Kids driving**: Majority have **0** (≈27K), tails at 1–3.
* **Claim Amount by Education × Marital** (totals):

  * **Divorced \$26.4M**, **Married \$50.6M**, **Separated \$14.5M**, **Single \$96.3M**.
  * Among Singles, **Bachelors \$38.7M** and **High School \$40.2M** dominate.

## Dashboard

* **Power BI file**: `Insurance_Risk_Claims.pbix`

## How to Run this project?

1. Clone the repo.
2. Open `Insurance_Risk_Claims.pbix` in **Power BI Desktop**.
3. If prompted, update data source paths for the CSV/Excel files in **Transform Data → Data source settings**.
4. Click **Refresh** to load data.
5. Use the **Select measures** slicer to switch the metric across visuals.

## Results & Conclusion

The dashboard highlights a private-use, mid-age, education-skewed portfolio with concentrated claim amounts among **Single** customers—especially **Bachelors** and **High School**—and reveals brand/zone segments for targeted action.

## Future Work

* Add **loss ratio** and **severity/frequency** per segment
* Create **alerts** for unusual spikes by car make/zone
* Add **drill-through** pages for claim details and policy cohorts

## Author & Contact

* **Author**: Ankita Basu
* **LinkedIn**: www.linkedin.com/in/ankita-basu-a7b0b628b
* **Email**: ankita16basu@gmail.com
