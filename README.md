# Healthcare Claims Denial Analysis

## Overview
Analysis of 8,000 healthcare insurance claims to identify denial patterns, quantify revenue loss, and uncover the root causes behind claim denials. Built using SQL for data analysis and Power BI for interactive visualization.

## Dataset
- **Size:** 8,000 claims
- **Columns:** 19 (claim ID, payer, specialty, claim status, billed amount, paid amount, denial reason, prior authorization status, CPT codes, service dates, and more)
- **Payers covered:** Medicare, Medicaid, and 3 major private insurers

## Tools Used
- **SQL (PostgreSQL)** — data querying and aggregation
- **Power BI** — interactive dashboard and DAX measures

## Key Findings
- **Overall denial rate: 21.6%** across all claims
- **Medicare has the highest denial rate at ~26%**, notably above other payers
- **Top denial reason: missing prior authorization**, responsible for **$1.05M** in lost revenue
- Claims without prior authorization obtained were denied at a dramatically higher rate than those with it

## Dashboard
The Power BI dashboard (`healthcare_claims_dashboard.pbix`) includes:
- Total Claims card (8,000)
- Denial Rate % card (21.6%)
- Clustered bar chart: denial rate by payer
- Donut chart: breakdown of denial reasons

![Dashboard Screenshot](dashboard_screenshot.png)

## SQL Analysis
The `healthcare_claims_sql_queries.sql` file contains 10 queries covering:
- Overall denial statistics
- Denial rate by payer
- Top 10 denial reasons by revenue impact
- Prior authorization impact on denial rate
- Denial rate by medical specialty
- High-risk payer-specialty combinations
- CPT code denial analysis
- Monthly revenue trends (paid vs. denied)

## Business Impact
These insights can guide a healthcare organization's revenue cycle team to prioritize prior authorization workflows and target payer-specific denial prevention strategies — directly reducing lost revenue.

## Author
Fatima Shirin — Data Analyst | Former Senior Process Executive, Medical Billing & Revenue Cycle Management
