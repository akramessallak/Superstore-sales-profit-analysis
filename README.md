#  Superstore Sales & Profit Performance Analysis

##  Executive Summary
This project delivers an interactive data analysis of the Global Superstore dataset built with **Microsoft Excel** (Pivot Tables, Dynamic Pivot Charts, Slicers, and Timelines). The objective is to evaluate revenue against profit across product categories, analyze regional performance, and identify key business risks.

---

##  Dashboard Overview & Key Visuals

### 1. Base Summary Data (Pivot Table)
The core numbers behind our analysis showing total sales and total profit per category:
![Pivot Table Overview](Screenshots/01_pivot_table_sales_vs_profit.png.png)

### 2. Sub-Category Deep-Dive & Discount Audit
Detailed breakdown analyzing the impact of average discounts and margins on product sub-categories:
![Sub-Category Audit](Screenshots/02_pivot_table_subcategory_deep_dive.png.png)

### 3. Global Performance by Category
Clean, formatted visual representation focused strictly on Core Metrics ($Sales vs$Profit across all regions):
![Global Sales vs Profit](Screenshots/03_sales_vs_profit_global_currency.png.png)

### 4. Interactive Slicers & Dynamic Filtering
Dynamic filtering tools configured for location (Region) and time (Timeline):
![Region Slicer and Timeline](Screenshots/04_slicers_region_and_timeline.png.png)

### 5. Regional Deep-Dive (Central Region Alert)
Filtering by the **Central Region** reveals critical margin loss in the Furniture line:
![Central Region Analysis](Screenshots/05_sales_vs_profit_central_region.png.png)

---

##  Key Findings & Business Insights

| Category | Total Sales ($) | Total Profit ($) | Profit Margin (%) | Performance Status |
| :--- | :--- | :--- | :--- | :--- |
| **Technology** | $836,154.03 | $145,454.95 | **~17.4%** | 🟢 High Performer |
| **Office Supplies** | $719,047.03 | $122,490.80 | **~17.0%** | 🟢 Stable |
| **Furniture** | $741,999.80 | $18,451.27 | **~2.5%** | 🔴 At-Risk Category |

* **Low Margin Alert:** **Furniture** generates heavy sales volume ($741.9K) but delivers an exceptionally low return ($18.4K).
* **Regional Loss:** In the **Central Region**, Furniture incurs an absolute loss of **-$2,871.05** on $163.7K of sales, driven by unoptimized discount structures.
* **Top Profit Engine:** **Technology** is the primary driver of profitability, yielding $145.5K in profit.

---

##  Strategic Recommendations

1. **Discount Cap Policy:** Restrict maximum allowable discounts on Furniture products (specifically *Tables* and *Bookcases*) to a maximum threshold of 15%.
2. **Regional Price Adjustment:** Re-evaluate regional pricing strategies in the **Central** zone to prevent negative margin orders.
3. **Invest in High-Margin Segments:** Reallocate promotional and advertising resources toward high-yield products in the **Technology** category.

---

##  Repository Structure

```text
superstore-sales-profit-analysis/
├── data/
│   └── Superstore_Dataset.xlsx
├── dashboards/
│   └── Superstore_Dashboard.xlsx
├── screenshots/
│   ├── 01_pivot_table_sales_vs_profit.png.png
│   ├── 02_pivot_table_subcategory_deep_dive.png.png
│   ├── 03_sales_vs_profit_global_currency.png.png
│   ├── 04_slicers_region_and_timeline.png.png
│   └── 05_sales_vs_profit_central_region.png.png
└── README.md
