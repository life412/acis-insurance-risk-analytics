# ACIS End-to-End Insurance Risk Analytics (Feb 2014 – Aug 2015)

## Business Objective
Identify low-risk customer segments and support risk-based pricing decisions (premium optimization) for AlphaCare Insurance Solutions (ACIS) in South Africa.

## What’s included (this week / Task 1)
- Data understanding and quality assessment
- Exploratory Data Analysis (EDA) for risk and profitability signals
- Initial insights to guide segmentation and later modeling (Tasks 3–4)

## Repository structure
- `data/` – raw and (later) versioned datasets
- `notebooks/` – EDA notebooks (profiling + visual insights)
- `src/` – reusable data loading, cleaning, and analysis utilities
- `reports/` – exported plots and analysis summaries
- `docs/` – assumptions, definitions, and methodology notes

## Key metrics (risk & profitability)
- Loss Ratio = TotalClaims / TotalPremium
- Claim Frequency = P(At least one claim | policy)
- Claim Severity = E[TOTALClaims | claim occurred]
- Margin = TotalPremium - TotalClaims

## How to run (baseline)
1. Install requirements: `pip install -r requirements.txt`
2. Run EDA notebook: `notebooks/01_eda.ipynb`

## Milestones (Task 1 deliverables)
- Data summary + quality checks (missingness, types)
- Distributions + outlier detection (TotalClaims, CustomValueEstimate, etc.)
- Geography & segment comparisons (Province, VehicleType, Gender)
- 3 high-quality visual insights (saved to `reports/figures/`)
