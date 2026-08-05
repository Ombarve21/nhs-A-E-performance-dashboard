# NHS A&E performance dashboard
NHS A&amp;E performance analysis and Power BI dashboard using Power Query and DAX.

An interactive Power BI dashboard analysing NHS England Accident & Emergency
performance from 2021 to 2024, tracking attendances, admissions, and
performance against the national four-hour A&E standard across trusts and
regions.

![Overview](images/overview_page.png)

## Project Overview

England's A&E departments are measured against a national standard: 95% of
patients should be admitted, transferred, or discharged within four hours of
arrival. This dashboard explores how far actual performance sits below that
target, which providers are under the most pressure, and how attendances and
admissions have changed over time.

## Key Findings

- Four-hour performance reached only **69%**, a **26-point gap** below the NHS
  95% operational standard.
- A&E attendances grew steadily from **22.8M (2021) to 27.4M (2024)**.
- The number of patients waiting more than four hours rose sharply year on year.
- Provider-level analysis highlights the trusts under the greatest pressure.

## Dashboard Pages

**1. A&E Overview** — headline KPIs (attendances, % seen in four hours, % seen
after four hours, emergency admissions), attendance trend, four-hour
performance by department type, and provider rankings.

**2. Emergency Admissions** — admissions trend, department-type breakdown, and
admissions by provider.

## Tools & Techniques

- **Power BI** — data model, report design, interactivity
- **Power Query** — data cleaning and transformation: flattening multi-row
  headers, unpivoting department-type columns, handling part-year data
- **DAX** — measures for four-hour compliance %, year-over-year change, and a
  dynamic KPI toggle
- **Data modelling** — star schema with a dedicated date dimension

## Data Cleaning Notes

The raw NHS spreadsheets required real preparation before analysis:

- Multi-row merged headers were flattened into single, usable column names.
- Department-type columns were unpivoted into an analysis-ready structure.
- 2025 data was part-year only, so it was excluded from trend visuals to avoid
  a misleading drop while keeping the year-on-year figures comparable.

## Data Source

NHS England Accident & Emergency Attendances and Emergency Admissions,
published under the Open Government Licence.
[NHS England A&E statistics](https://www.england.nhs.uk/statistics/statistical-work-areas/ae-waiting-times-and-activity/)

## Author

Om Barve — MSc Data Science, University of Sheffield
[LinkedIn](https://www.linkedin.com/in/contactombarve) ·
[GitHub](https://github.com/Ombarve21)
