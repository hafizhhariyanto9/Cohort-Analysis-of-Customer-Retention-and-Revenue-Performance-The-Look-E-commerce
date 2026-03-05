# Cohort Analysis: Customer Retention & Revenue Performance on The Look

## Overview
This project analyzes cohort-based customer retention and revenue retention for **The Look**, a global fashion e-commerce platform. The goal is to understand how well the platform retains customers and revenue across cohorts from 2019 to 2024.

## Problem Statement
How do customer retention and revenue retention patterns differ across cohorts (2019–2024), and which cohorts show the most sustainable performance to support business growth strategy?

## Objectives
1. Analyze revenue retention patterns for each customer cohort (2019–2024)
2. Identify cohorts with the most sustainable long-term revenue contribution
3. Evaluate retention trend changes before, during, and after the pandemic
4. Provide data-driven insights for retention and promotion strategies

## Dataset
- **Source:** `order_items.csv` — The Look e-commerce transaction data
- **Period:** January 2019 – January 2024
- **Size:** 181,759 rows
- **Key columns:** `user_id`, `created_at`, `sale_price`, `status`

## Methodology
- **Cohort grouping:** by semester (S1 = Jan–Jun, S2 = Jul–Dec)
- **Retention metrics:** Customer Retention Rate & Revenue Retention Rate
- **Visualizations:** Heatmap & Lineplot per cohort

## Key Findings

**Customer Retention:**
- All cohorts experience a steep drop from 100% at S0 to only **2–7% at S1**
- Best performing cohort at S1: **2023-S1 (6.98%)**, followed by 2022-S2 (4.93%)
- After S1, retention stabilizes at **1–5%** consistently across all cohorts
- Newer cohorts (2022–2023) show improved S1 retention vs older ones (2019–2021)

**Revenue Retention:**
- Mirrors customer retention closely with **85–90% correlation**
- Revenue retention is generally **0.1–0.3% higher** than customer retention — retained customers tend to spend more
- Highest S1 revenue retention: **2023-S1 (7.19%)**
- Long-tail revenue observed — cohort 2019-S2 still contributes revenue through semester 8

## Strategic Recommendations
1. **Prioritize S1 retention** — it's the critical bottleneck and has the highest ROI impact
2. **Repeat purchase program** — offer vouchers/free shipping for 2nd purchase to push S1 retention from ~5% → 8%
3. **Monitor revenue vs customer retention gap** — healthy gap = 0.2–0.5%; alert if it turns negative
4. **Replicate 2023-S1 strategy** — this cohort had the best performance; build a playbook from it
5. **Analyze long-surviving customers** (2019-S2) — identify product and pricing factors that drive longevity

## Tools & Libraries
- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Google BigQuery (TheLook dataset)
