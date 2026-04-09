# AWS SaaS Sales Performance Analysis: Identifying Profit Loss Drivers in Japan (2020–2023)

#### Created by Indira Faisa Afgani for the 2nd Capstone Project - Data Science and Machine Learning Program
---

## Project Overview
This project analyzes AWS SaaS sales transaction data to identify the root causes of profit losses in the APJ region, specifically in Japan. Despite being the top revenue generator in the region with $170,188 in sales, Japan recorded a total loss of -$25,729. This analysis aims to uncover the factors driving these losses and provide actionable business recommendations.

---

## Problem Statement
AWS SaaS recorded consistent profit growth overall, yet the APJ region, particularly Japan, has generated a total loss of -$25,729 despite being the top revenue generator in the region.

This analysis aims to answer the following questions:

1. Where do the largest losses occur, and which products contribute the most?
2. What causes those products to be unprofitable in Japan, and what recommendations can be made to address the losses?

---

## Dataset
- **Source**: AWS SaaS Sales Dataset
- **Period**: 2020 – 2023
- **Size**: 9,994 rows × 19 columns
- **Type**: B2B SaaS sales transactions across 3 regions: EMEA, AMER, APJ

---

## Tools & Libraries
- **Python** (Jupyter Notebook)
- **Pandas** — data manipulation
- **NumPy** — numerical operations
- **Matplotlib & Seaborn** — data visualization
- **Plotly** — interactive charts
- **Folium** — geographical map visualization
- **Tableau Public** — interactive dashboard

---

## Analysis Structure
1. **Basic Data Understanding** — exploring data structure, types, and statistics
2. **Data Cleaning** — fixing datatypes, handling duplicates, missing values, consistency checks, and outliers
3. **Exploratory Data Analysis (EDA)**
   - Profit Distribution
   - Discount Distribution
   - Correlation Matrix
4. **Yearly Trend** — sales and profit performance from 2020 to 2023
5. **Geographical Analysis**
   - Region → APJ identified as lowest profit region
   - Subregion → JAPN identified as the most problematic subregion
   - Country → Japan confirmed as the main source of losses
6. **Analyzing the Cause**
   - Product Analysis → ContactMatcher as the biggest loss driver
   - Discount Analysis → excessive discounting identified as root cause
   - Global vs Japan Comparison → discount anomaly confirmed as Japan-specific
   - Discount and Profit Summary → only ≤20% discount generates profit in Japan
7. **Business Recommendation** — actionable insights based on findings

---

## Key Findings
- Japan has the **highest sales in APJ ($170k)**. However, the country records the **largest loss (-$25,729)**
- **ContactMatcher** is the primary loss driver, accounting for over 65% of Japan's total losses (-$16,922)
- Japan applies an average discount of **71%** for Contactmatcher vs only **31%** globally
- Contactmatcher is **profitable outside Japan**, proving the product itself is not the issue
- Only discounts **≤20%** generate profit in Japan — all higher discount levels result in losses without exception

---

## Business Recommendations
1. **Limit the maximum discount for Contactmatcher in Japan at 20%** — the only discount level proven to generate profit
2. **Audit internal discount approval process** — investigate why 80% discounts are being approved in Japan
3. **Use profitable products as benchmark** — Site Analytics, Support, and Data Smasher maintain profit with only 20% discount

---

## Files
| File | Description |
|------|-------------|
| `Capstone_2_Clean_Version.ipynb` | Main analysis notebook |
| `SaaS-Sales.csv` | Original dataset |
| `SaaS-Sales-Cleaned.csv` | Cleaned dataset after preprocessing |
| `Capstone 2 - AWS SaaS Sales - Indira Faisa Afgani` | Canva presentation of the analysis |

---

## Links
- **Tableau Dashboard**: https://public.tableau.com/app/profile/indira.afgani/viz/AWSSaaSSalesDashboard-IndiraFaisaAfgani/Dashboard1?publish=yes
- **Presentation**: https://canva.link/f02ekbt61fuw2wm