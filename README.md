# Superstore Business Intelligence Capstone 📊🍷

## 📌 Project Overview
An enterprise-grade Power BI dashboard engineered to transition a retail business from volume-driven sales to profit-led scaling. This project replaces vanity metrics with actionable data models, focusing on cross-selling optimization, unit economics, and targeted customer retention.

### 🗂️ Repository Structure
```text
Superstore-Business-Intelligence-Capstone/
├── README.md
├── Superstore_Executive_Hub.pbix
├── Superstore_Capstone_Dashboard_Export.pdf
├── Superstore_Capstone_Proposal.pdf
├── Superstore_Project_Theme.json
```

## 📊 Analytical Engines & Key Insights

### 1. Executive Overview & Top-Line Performance
* **The Reality:** While top-line revenue and order volumes appear strong, they act as vanity metrics that mask severe underlying margin leaks.
* **The Fix:** Shifted the analytical focus away from gross sales and toward net profit capture and structural margin governance.

### 2. Cross-Selling Engine (FP-Growth Model)
* **The Architecture:** Utilizes a custom DAX-driven Market Basket Analysis based on the FP-Growth algorithm to identify hidden purchasing relationships.
* **The Insight:** High-confidence natural pairings exist (e.g., Technology and Furnishings). Hardcoding these specific product recommendations into the checkout flow organically increases Average Order Value (AOV) without relying on margin-destroying discounts.

### 3. Profitability & Portfolio Strategy
* **The Architecture:** A unit economics audit combined with a dynamic DAX discount sensitivity curve locked to a secondary axis.
* **The Insight:** Furniture items (specifically Tables and Bookcases) are structural loss leaders. The sensitivity model mathematically proves that any promotional discount exceeding **20%** causes net profit margins to collapse completely into negative territory.
* **Action:** Establish a strict 20% discount cap. Reprice, bundle, or delist capital-destroying products.

### 4. Customer Retention & RFM Engine
* **The Architecture:** A behavioral segmentation model built using the `ADDCOLUMNS` and `SWITCH` DAX functions. It calculates Recency, Frequency, and Monetary value across the entire customer lifecycle to assign dynamic marketing tiers.
* **The Insight:** A small segment of "Champions" carries the enterprise, while a high volume of previously valuable customers are slipping into the "At Risk" tier.
* **Action:** Halt expensive blanket marketing. Redirect the promotional budget specifically to win-back campaigns targeting the actionable "At Risk" matrix hit-list.

## 🎨 Design & UI Architecture
* **Theme:** Custom JSON theme applying a Wine Red (`#7F011F`), Light Sand (`#F5EBD0`), and Deep Slate (`#2C3E50`) palette.
* **UX:** Designed with 10px rounded borders, clean center-aligned matrices, and dynamic slicers to provide a cohesive, modern app-like executive experience.

## 📂 File Descriptions
* `Superstore_Executive_Hub.pbix`: The complete Power BI project file containing all Power Query M code, DAX measures, and data models.
* `Superstore_Capstone_Proposal.pdf`: The initial project scoping document outlining the business problem, dataset, and planned analytical architecture.
* `Superstore_Project_Theme.json`: The custom structural theme file.

---
*Built to demonstrate advanced data engineering, DAX proficiency, and strategic business analysis.*
