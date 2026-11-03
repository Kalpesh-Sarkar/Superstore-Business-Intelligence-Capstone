# Superstore Business Intelligence Capstone 📊🍷

## Project Overview
This repository contains an enterprise-grade Business Intelligence architecture built for a simulated retail entity, "Superstore". The primary objective of this capstone was to transition the company's operational strategy from volume-driven vanity metrics (gross sales) to a sustainable, profit-led growth model.

**Tech Stack:** Power BI, DAX, Power Query (M), JSON (Custom UI Architecture)  
**Core Analytical Models:** FP-Growth (Market Basket), RFM Segmentation, Unit Economics & Breakeven Analysis

---

## 🛠️ Data Architecture & ETL
The foundation of this project was built on a raw, highly disconnected dataset (`Superstore_Messy`). To ensure enterprise-grade accuracy, extensive data engineering was performed:
* **Data Cleansing (Power Query):** Stripped invalid strings (e.g., "Unknown Customer"), standardized datetime formats, and resolved null financial anomalies.
* **Custom DAX Engines:** Engineered fully customized, disconnected analytical tables to bypass standard star-schema limitations. This includes a dedicated Cross-Selling matrix and a dynamic Customer_RFM table generated via `ADDCOLUMNS` and nested `SWITCH` statements.
* **UI/UX Design:** Built a completely custom JSON theme utilizing a Wine Red (`#7F011F`), Light Sand (`#F5EBD0`), and Deep Slate (`#2C3E50`) palette to deliver a modern, app-like executive experience.

---

## 📈 The 4 Analytical Engines (Dashboard Pages)

### 1. Executive Overview: The "Vanity Metric" Trap
At first glance, top-line historical data (2011–2018) shows massive order volume and gross revenue. However, the dashboard reveals that overall revenue acts as a vanity metric. Massive spikes in sales volume frequently correlate with drops in net profit, indicating severe margin leaks hidden beneath promotional growth.

### 2. Cross-Selling Engine (FP-Growth Model)
To increase Average Order Value (AOV) without relying on discounts, I implemented an FP-Growth Market Basket Analysis model. 
* **Insight:** The DAX engine mathematically calculates "Bundle Confidence" (conditional probability). For example, it identifies the exact percentage likelihood that a customer buying a Phone will also purchase Storage.
* **Action:** Hardcoding these high-confidence product pairings into the online checkout flow drives organic, highly profitable cross-selling.

### 3. Profitability & Portfolio Strategy (Unit Economics)
This engine audits the product portfolio to isolate "Capital Destroyers" (structural loss leaders like Tables and Bookcases). 
* **Insight:** I engineered a custom dynamic DAX threshold line on the secondary axis of the discount sensitivity curve. It mathematically proves that **any promotional discount exceeding 20% causes net profit margins to collapse completely into negative territory**, regardless of the volume sold.

### 4. Customer Retention & RFM Engine
Rather than relying on demographic assumptions or simple year-by-year slicing, this engine uses RFM (Recency, Frequency, Monetary) behavior to evaluate true lifetime customer value.
* **Insight:** The DAX model dynamically assigns every customer a composite score and categorizes them into marketing tiers (e.g., 🏆 Champions, ⚠️ At Risk). 
* **Action:** Leadership can instantly filter the database to generate a targeted hit-list of high-value "At Risk" customers, redirecting blanket marketing budgets toward highly efficient win-back campaigns.

---

## 💡 Strategic Executive Recommendations
Based on the data architecture and models built in this dashboard, the "Bull Case" for Superstore requires three immediate operational shifts:
1. **Enforce a Strict 20% Discount Cap:** Implement strict pricing governance; no standard promotional discount can exceed the 20% breakeven threshold.
2. **Restructure Loss Leaders:** Discontinue structurally unprofitable items (Tables/Bookcases) or gate them exclusively behind high-margin bundles using the Page 2 cross-selling engine.
3. **Targeted Retention Marketing:** Cease uncalibrated, blanket marketing. Reallocate the promotional budget exclusively toward the "At Risk" RFM segment to maximize ROI.
