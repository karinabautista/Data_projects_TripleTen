# Website Conversion & Retention Analysis
An Excel-based analysis of website user behavior, focusing on conversion funnels and retention cohorts over a 4-month period (Sep 2020 – Feb 2021). This project provides insights into how users progress through the purchase journey and how retention varies across cohorts.

## Project Overview

- Time Period: Late September 2020 – February 2021
- Data Source: Website activity logs (each row represents a user action)
- Objective: Analyze user behavior to:
- Understand the conversion funnel from site visit to purchase
- Measure cohort-based retention rates

## Key Findings
| Metric | Insight |
| ----------- |----------- |
| Conversion Funnel |	Total site conversion is 10%, but cart-to-purchase conversion is 35%, showing a 25-point jump. Users who pass the initial intent barrier are highly likely to complete a purchase. |
| Retention Rates |	The September 2020 cohort had the highest retention over the 4 months. All cohorts exhibit a gradual daily decay in repeat purchases. |

## Analysis / Methods
| Component |	Description |
|------| ----- |
| Raw Data |	Each row represents a user action, with fields: user ID, event type, and event date. Analysis focuses on these fields to define cohorts and construct conversion funnels. |
| Conversion Funnel |	Two metrics were used:<br> 1. **Total Conversion:** % of unique users reaching a stage from the initial visit<br> 2. **Step-to-Step Conversion:** % of users progressing from one stage to the next |
| Retention Rates |	Cohorts defined by the first purchase month. Monthly retention calculated as % of users making repeat purchases relative to the original cohort size. |

## Visualizations
