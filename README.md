# Uber Trip Analysis Dashboard (Tableau)

<p align="left">
  <img src="https://img.shields.io/badge/Focus-Data%20Analytics-111111?style=for-the-badge" alt="Focus Data Analytics" />
  <img src="https://img.shields.io/badge/Domain-Uber%20Trips-276EF1?style=for-the-badge" alt="Domain Uber Trips" />
  <img src="https://img.shields.io/badge/Status-Portfolio%20Project-12B886?style=for-the-badge" alt="Status Portfolio Project" />
</p>

An end-to-end, dashboard-first analysis of Uber trip activity built to answer **when to drive, what to drive, and where revenue clusters**.

## Tech Stack

<p align="left">
  <img src="https://skillicons.dev/icons?i=python" alt="Python" />
  <img src="https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white" alt="Tableau" />
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel" />
  <img src="https://img.shields.io/badge/Git-GitHub%20Workflow-181717?style=for-the-badge&logo=github&logoColor=white" alt="Git and GitHub" />
</p>

## What you’ll find here

- **An interactive Tableau dashboard** for exploring revenue, demand, category mix, and route concentration
- **Static chart exports** (PNG) so the repo is reviewable even without Tableau
- **A compact metrics snapshot** and “so what?” insights, written for business stakeholders

## Quick preview (what recruiters will scan)

<img width="1260" alt="Dashboard preview" src="./charts/Dashboard01.png" />

## Dataset snapshot

From the `REAL ROUTES` sheet in `UBER_RAW.xlsx` (721 usable trip rows after excluding incomplete exports):

- **Total revenue**: `R$11,535.34`
- **Average fare / trip**: `R$16.00`
- **Average distance**: `5.14 km`
- **Average duration**: `12.53 min`

## Key insights (TL;DR)

- **Demand + revenue stack up in daytime and early evening**, where trip volume stays consistently high.
- **`Comfort` dominates** this dataset in both trip count and revenue contribution.
- **Revenue concentrates into repeat routes**, suggesting strong neighborhood-based demand clustering.
- **Fast review experience**: chart exports make this repo scannable in under 2 minutes.

## Chart gallery

### 1) Hourly revenue vs. trip volume

<img width="1000" alt="Hourly revenue and trips" src="./charts/hourly_revenue_trips.png" />

### 2) Revenue by ride category

<img width="900" alt="Revenue by ride category" src="./charts/revenue_by_category.png" />

### 3) Top routes by revenue

<img width="1000" alt="Top routes by revenue" src="./charts/top_routes_revenue.png" />

## Business questions answered

- **When to drive**: which hours combine high revenue with high trip volume?
- **What to drive**: which ride categories contribute most to earnings?
- **Where value concentrates**: which pickup → dropoff pairs generate the strongest returns?
- **Consistency**: how stable are patterns across seasons and neighborhoods?
- **Efficiency**: where can time and distance be optimized without reducing revenue?

## Method (high-level)

- **Normalize money values** from currency-formatted strings (e.g., `R$47.81`)
- **Convert duration and distance** into numeric values suitable for aggregation
- **Standardize pickup/dropoff labels** for reliable route grouping
- **Filter duplicates / incomplete exports** prior to visualization and chart generation

## Tools

- **Tableau**: dashboard design + interactive analysis (`UBER dashboard.twb`)
- **Excel**: raw + cleaned workbooks (`UBER_RAW.xlsx`, `UBER_Clean.xlsx`)
- **Python**: generation of static chart exports stored under `charts/`

## Repo layout

- `README.md`: this page
- `UBER dashboard.twb`: Tableau workbook (interactive dashboard)
- `UBER_RAW.xlsx`: source workbook containing raw/reference sheets
- `UBER_Clean.xlsx`: cleaned workbook for analysis
- `charts/`: dashboard screenshot + static chart exports used above

## How to review (recommended)

1. **Start here**: scan the dashboard preview + the 3 charts.
2. **Open Tableau**: load `UBER dashboard.twb` to explore filters and drill-downs.
3. **Audit the data**: inspect `UBER_RAW.xlsx` / `UBER_Clean.xlsx`.

