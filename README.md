#  Superstore Sales & Profit Performance Analysis

##  Executive Summary
This project delivers an interactive data analysis of the Global Superstore dataset built with **Microsoft Excel** (Pivot Tables, Dynamic Pivot Charts, Slicers, and Timelines). The objective is to evaluate revenue against profit across product categories, analyze regional performance, and identify key business risks.

---

##  Dashboard Overview & Key Visuals

### 1. Base Summary Data (Pivot Table)
The core numbers behind our analysis showing total sales and total profit per category:
![Pivot Table Overview](Screenshots/01_pivot_table_sales_vs_profit.png.png)
Le Problème Majeur : Furniture génère un énorme chiffre d'affaires (742k$), mais ne rapporte presque RIEN en profit (18.4k$) par rapport aux autres ! Pourquoi ? C'est ce qu'on va découvrir grâce aux remises (Discount).

### 2. Sub-Category Deep-Dive & Discount Audit
Detailed breakdown analyzing the impact of average discounts and margins on product sub-categories:
![Sub-Category Audit](Screenshots/02_pivot_table_subcategory_deep_dive.png.png)
Dès qu'une sous-catégorie dépasse 20% de Discount moyen (Tables, Bookcases, Binders), sa marge moyenne devient négative !

### 3. Global Performance by Category
Clean, formatted visual representation focused strictly on Core Metrics ($Sales vs$Profit across all regions):
![Global Sales vs Profit](Screenshots/03_sales_vs_profit_global_currency.png.png)
Furniture : La barre bleue (Sales) est énorme, mais la barre orange (Profit) est presque au sol (à peine visible) !
Office Supplies & Technology : Les barres oranges sont bien hautes et en bonne santé.

### 4. Interactive Slicers & Dynamic Filtering
Dynamic filtering tools configured for location (Region) and time (Timeline):
![Region Slicer and Timeline](Screenshots/04_slicers_region_and_timeline.png.png)
Si je cliques sur la région Central dans le Slicer, que devient le profit pour la catégorie Furniture ? Est-ce qu'il est positif ou négatif ?

### 5. Regional Deep-Dive (Central Region Alert)
Filtering by the **Central Region** reveals critical margin loss in the Furniture line:
![Central Region Analysis](Screenshots/05_sales_vs_profit_central_region.png.png)
Furniture fait un profit négatif de $(2,871.05) !
Technology est en tête avec $33,697.43 de profit !
Filtering by the Central Region exposes a major financial drain in the Furniture department:
While overall revenue in the Central zone remains solid, Furniture generates a net loss of -$2,871.05 due to localized over-discounting.

##  6. Discount & Profitability Analysis

An analysis of discount levels reveals the primary root cause of losses in the **Furniture** category:

* **0% – 20% Discount:** Products remain profitable, generating healthy margins.
* **> 20% Discount (Tipping Point):** Any discount exceeding **20%** causes immediate, significant financial losses (plunging to **-$10,695.32** at 30% discount).

>  Heavy discounting on Furniture items completely destroys product margins. 

![Furniture Discount Analysis](Screenshots/06_furniture_discount_analysis.png.png)

##  7. Top vs. Bottom Product Performance
A deep dive into individual product profitability reveals extreme disparities:
![Top and Flop Products Analysis](Screenshots/07_top_flop_products.png)
High-ticket items like 3D printers and large conference tables suffer massive losses when paired with aggressive discounting (>20%). Conversely, copiers and office binding equipment represent our most lucrative lines.

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

Based on the quantitative findings from the Superstore dataset analysis, we recommend implementing the following **4 key business actions**:

### 1. 🛑 Enforce a Hard Cap on Discounts (>20%)
* **Problem:** Data proves that any discount over **20%** severely destroys profitability, resulting in net losses as deep as **-$16,187.40** (at 40% discount).
* **Action:** Restrict sales representative authorization for discounts. Any discount exceeding **15%** should require manager approval, with a **hard limit at 20% max**.

### 2. 🛋️ Restructure Furniture Category Pricing
* **Problem:** Heavy items like *Conference Tables* (e.g., Chromcraft & Bush Advantage lines) incur major losses due to combined high shipping costs and aggressive discounting.
* **Action:** Re-evaluate shipping fees for bulk furniture items and eliminate discount promotions on heavy office tables.

### 3. 🖨️ Audit High-Loss Technology Items
* **Problem:** Products like the *Cubify CubeX 3D Printers* generated massive losses exceeding **-$12,000** combined.
* **Action:** Review supplier pricing, warranty costs, or discontinue stocking non-performing items like 3D printers that suffer from high return/discount rates.

### 4. 📈 Double Down on Top Performers
* **Problem:** Office Copiers and Binding Machines generate exceptional profits (e.g., *Canon imageCLASS 2200* alone generated **+$25,199.93**).
* **Action:** Increase marketing spend and bundle promotions around high-margin technology assets (Copiers & Laserjet lines).

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
