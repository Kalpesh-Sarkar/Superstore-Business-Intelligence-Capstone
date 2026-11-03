# ⚡ Superstore Business Intelligence Capstone

![BI Tool](https://img.shields.io/badge/BI_TOOL-POWER_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Engine](https://img.shields.io/badge/ENGINE-DAX-0078D4?style=for-the-badge)
![ETL](https://img.shields.io/badge/ETL-POWER_QUERY-yellow?style=for-the-badge)
![Algorithm](https://img.shields.io/badge/ALGORITHM-FP--GROWTH-blue?style=for-the-badge)
![License](https://img.shields.io/badge/LICENSE-MIT-green?style=for-the-badge)

> An enterprise-grade Power BI dashboard engineered to transition a retail business from volume-driven sales to profit-led scaling. This project replaces vanity metrics with actionable data models, focusing on cross-selling optimization, unit economics, and targeted customer retention.

## 📑 Table of Contents

* [Analytical Engines & Key Insights](#-analytical-engines--key-insights)
* [Design & UI Architecture](#-design--ui-architecture)
* [Repository Contents](#-repository-contents)

## 📊 Analytical Engines & Key Insights

### 1. Executive Overview & Top-Line Performance
* **The Reality:** While top-line revenue and order volumes appear strong, they act as vanity metrics that mask severe underlying margin leaks.
* **The Fix:** Shifted the analytical focus away from gross sales and toward net profit capture and structural margin governance.

### 2. Cross-Selling Engine (FP-Growth Model)
* **The Architecture:** Utilizes a custom DAX-driven Market Basket Analysis based on the FP-Growth algorithm to identify hidden purchasing relationships.
* **The Insight:** High-confidence natural pairings exist (e.g., Technology and Furnishings). Hardcoding these specific product recommendations into the checkout flow organically increases Average Order Value (AOV) without relying on margin-destroying discounts.

### 3. Profitability & Portfolio Strategy
* **The Architecture:** A unit economics audit combined with a dynamic DAX discount sensitivity curve locked to a secondary axis.
* **The Insight:** Furniture items (specifically Tables and Bookcases) are structural loss leaders. The sensitivity model mathematically proves that any promotional discount exceeding **20%** causes net profit
