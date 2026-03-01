# Sales & Customer Dashboard w/ Tableau

![Sales Dashboard](/Sales_Customer_Dashboard/images/sales_dashboard.png)

[🌐 **View Interactive Dashboard on Tableau Public**](https://public.tableau.com/shared/T3MMYJ232?:display_count=n&:origin=viz_share_link)

## Introduction

This project was built to provide **Sales Managers, Business Analysts, and Executive Stakeholders** with a clear, interactive view of key business metrics. Using a structured dataset of orders, customers, and product data spanning **EU and Non-EU regions**, this Tableau project delivers two dedicated dashboards — one focused on **Sales & Profit performance**, and the other on **Customer behavior & segmentation** — enabling users to quickly identify trends, spot outliers, and drive smarter decisions.

### Dashboard File
You can find the Tableau workbook file here: [`Sales_Customer_Dashboard.twbx`](Sales_Customer_Dashboard.twbx).

## Data Sources

The project uses **CSV datasets** organized by region, each containing four core tables:

```
datasets/
├── eu/
│   ├── Customers.csv
│   ├── Location.csv
│   ├── Orders.csv
│   └── Products.csv
└── non-eu/
    ├── Customers.csv
    ├── Location.csv
    ├── Orders.csv
    └── Products.csv
```

| Table | Description |
|-------|-------------|
| **Customers** | Customer demographics and identifiers |
| **Location** | Geographic data for regional analysis |
| **Orders** | Transactional order data including sales, profit, and quantity |
| **Products** | Product catalog with categories and subcategories |

The EU and Non-EU datasets are **unioned** within Tableau to create a single, comprehensive global view of the business.

## Assets

The [`icons/`](icons/) folder contains custom navigation and filter icons used throughout the dashboard to provide a polished, app-like user experience — including icons for switching between the Sales and Customer views and toggling the filter panel.

## Skills Showcased

This project was a journey through key Tableau features. Here's a look at what was mastered:

-   **🎨 Dashboard Design & UX:** Designed a clean, professional layout with a consistent color scheme (orange, blue, grey) and intuitive custom navigation icons to switch between the Sales and Customer views.
-   **⚙️ Data Preparation & Union:** Connected and unioned multiple regional CSV datasets (EU & Non-EU) to build a unified data source across four core tables (Customers, Location, Orders, Products).
-   **🧮 Calculated Fields & Table Calculations:** Built custom calculations for Year-over-Year (YoY) comparisons, profit/loss classification, and customer ranking metrics.
-   **📈 KPI Cards with Sparklines:** Created summary KPI cards showing current-year totals with YoY % change and embedded sparkline trend lines highlighting the highest and lowest months.
-   **📊 Combo Charts (Bar + Trend Overlay):** Used horizontal bar charts with overlaid profit/loss indicators to compare **Sales & Profit by Subcategory**, making it easy to spot underperforming categories like Tables.
-   **📉 Time-Series Analysis:** Built **Sales & Profit Trends over Time** charts using step/line charts with color-coded above/below average thresholds, clearly distinguishing strong and weak performance periods.
-   **📋 Ranked Data Tables:** Constructed a **Top 10 Customers by Profit** table with rank, last order date, profit, sales, and order count — providing a quick executive summary of the most valuable customers.
-   **📊 Distribution Analysis:** Created a **Customer Distribution by Nr. of Orders** histogram to understand purchasing frequency patterns across the customer base.
-   **🖱️ Interactive Features:**
    -   **Filters:** Dynamic filtering by year, category, and other dimensions.
    -   **Custom Navigation Icons:** Icon-based buttons (from the [`icons/`](icons/) folder) to seamlessly switch between the Sales Dashboard and Customer Dashboard.
    -   **Filter Panel:** A dedicated filter icon to toggle advanced filtering options.

---

## Dashboard Overview

*This project is split into two dedicated dashboards to provide focused, role-specific insights.*

### Dashboard 1: Sales Dashboard | 2023

![Sales Dashboard](/Sales_Customer_Dashboard/images/sales_dashboard.png)

This is your command center for sales performance. At a glance, you can see:

| KPI | Value | YoY Change |
|-----|-------|------------|
| **Total Sales** | $733K | ▲ 20.4% vs. PY |
| **Total Profit** | $93K | ▲ 14.2% vs. PY |
| **Total Quantity** | $12K | ▲ 26.8% vs. PY |

Each KPI card includes a **sparkline** showing monthly trends, with the **highest month** (🔵) and **lowest month** (🟠) clearly marked.

The **Sales & Profit by Subcategory** chart breaks down performance across 17 product subcategories, instantly revealing that **Phones** and **Chairs** are top sellers, while **Tables** show a significant loss.

The **Sales & Profit Trends over Time** panel tracks weekly performance against the average, color-coding periods **above** (🔵 blue) and **below** (🟠 orange) the benchmark — a powerful way to identify seasonal patterns and anomalies.

### Dashboard 2: Customer Dashboard | 2023

![Customer Dashboard](/images/customer_dashboard.png)

This dashboard shifts the focus to customer behavior and segmentation:

| KPI | Value | YoY Change |
|-----|-------|------------|
| **Total Customers** | 693 | ▲ 8.6% vs. PY |
| **Total Sales Per Customer** | $1,058 | ▲ 10.8% vs. PY |
| **Total Orders** | 1,687 | ▲ 28.3% vs. PY |

The **Customer Distribution by Nr. of Orders** histogram reveals that most customers place 1–2 orders, with a steep drop-off — signaling opportunities for retention and repeat-purchase campaigns.

The **Top 10 Customers by Profit** table provides an executive-level view of the most profitable customers, with **Raymond Buch** leading at $6,781 in profit from just 3 orders, and **Hunter Lopez** close behind at $5,046 profit.

---

## Conclusion

This Tableau project demonstrates how interactive dashboards can transform raw transactional data from multiple regions into a powerful business intelligence tool. By separating sales performance from customer analytics into two dedicated views, stakeholders can quickly drill into the metrics that matter most to their role — whether it's identifying underperforming product categories, spotting seasonal trends, or recognizing the most valuable customers for targeted engagement.

[🌐 **Explore the Live Dashboard on Tableau Public →**](https://public.tableau.com/shared/T3MMYJ232?:display_count=n&:origin=viz_share_link)