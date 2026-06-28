# Retail Executive Dashboard & Data Storytelling

## Project Overview

This project presents an **Executive Retail Performance Dashboard** developed using Tableau to help business leaders monitor sales performance, profitability, customer behavior, shipping efficiency, discount effectiveness, and return patterns.

The dashboard consolidates multiple business metrics into a single interactive view, enabling executives to quickly identify trends, operational risks, and business opportunities for data-driven decision-making.

---

# Business Problem Summary

Retail leadership requires a centralized dashboard to answer key business questions, including:

* How is overall business performance changing over time?
* Which regions and product categories generate the highest revenue and profit?
* Which customer segments contribute the most value?
* How do discounts affect profitability?
* Which products experience the highest return rates?
* Are shipping operations meeting customer expectations?

The objective of this dashboard is to transform raw transactional data into meaningful business insights that support strategic decision-making.

---

# Dataset Description

The dashboard is built using the provided retail sales dataset (`dashboard_sales_data.xlsx`).

The dataset includes information related to:

* Orders
* Sales
* Profit
* Customers
* Product Categories
* Sub-Categories
* Shipping
* Discounts
* Returns
* Geographic Locations
* Order Dates

This information enables both high-level business monitoring and detailed operational analysis.

---

# Tableau Workbook Description

The Tableau workbook (`executive_dashboard.twbx`) contains:

* Executive Dashboard
* Supporting Worksheets
* Calculated Fields
* Dashboard Actions
* Parameter Actions
* Interactive Filters
* Viz in Tooltip
* Dashboard Navigation Components

The dashboard has been designed following executive reporting and data visualization best practices.

---

# Calculated Fields Created

Several calculated fields were created to support KPI calculations and business analysis.

Major calculated fields include:

* Current Year (CY) Sales
* Previous Year (PY) Sales
* Current Year Profit
* Previous Year Profit
* Current Year Orders
* Previous Year Orders
* Current Year Return Rate
* Previous Year Return Rate
* Year-over-Year Growth %
* Profit Margin
* Average Order Value (AOV)
* Return Rate
* Shipping Delay Bucket
* Dynamic Metric Selection (Sales / Profit / Orders)
* Reference Line Calculations

These calculations enable year-over-year comparison and interactive dashboard analysis.

---

# Dashboard Components

The dashboard contains the following analytical views:

### Executive KPI Cards

* Total Sales
* Total Profit
* Total Orders
* Return Rate

Each KPI displays:

* Current Year Value
* Previous Year Value
* Year-over-Year Growth
* Performance Indicator

---

### Sales Trend

A parameter-driven line chart allows users to dynamically switch between:

* Sales
* Profit
* Orders

to analyze monthly performance trends.

---

### Regional Performance

Horizontal bar chart comparing sales across regions with drill-down analysis using **Viz in Tooltip**.

---

### Category Profitability

Ranks product sub-categories based on profitability, helping identify top-performing and underperforming product groups.

---

### Shipping Performance

Displays:

* Average Delivery Days
* Order Distribution by Shipping Delay Bucket

to evaluate logistics performance.

---

### Customer Segment Performance

Executive scorecard comparing:

* Sales
* Profit Margin
* Average Order Value (AOV)

across customer segments.

---

### Discount Impact on Profitability

Scatter plot analyzing the relationship between discount percentage and profit.

Reference lines highlight average discount and average profit to identify profitable and loss-making transactions.

---

### Return Hotspots

Heatmap visualizing return rates across product categories and sub-categories.

Interactive tooltips display:

* Sales
* Profit
* Return Count
* Customer Segment Breakdown

---

# Filters and Dashboard Interactions

The dashboard includes several interactive features to improve usability.

### Global Filters

* Order Date
* Region
* Category
* Sub-Category
* Ship Mode
* Campaign Channel

---

### Interactive Features

* Parameter-driven metric selector
* Dashboard Action Filters
* Viz in Tooltip
* Reset Filters button
* Dynamic filtering across all visualizations

These features allow users to explore the dashboard while maintaining a consistent analytical context.

---

# Key Business Insights

Major insights obtained from the dashboard include:

* Sales and order volume have increased compared to the previous year.
* Profit growth is slower than revenue growth, indicating pressure on margins.
* Regional performance varies significantly, highlighting opportunities for targeted sales initiatives.
* Technology products contribute strong profitability, while several Furniture sub-categories require attention.
* Higher discount levels are associated with an increased number of loss-making orders.
* Most deliveries occur within the Normal shipping window, indicating stable logistics performance.
* Customer segment performance remains relatively balanced across all segments.
* Return hotspot analysis identifies product groups requiring further investigation to reduce operational costs.

---

# Dashboard Story Summary

The dashboard follows a structured analytical flow:

1. Executive KPI overview.
2. Business performance trend analysis.
3. Regional sales comparison.
4. Product profitability evaluation.
5. Shipping performance monitoring.
6. Customer segment comparison.
7. Discount impact analysis.
8. Return hotspot identification.

This progression enables executives to move naturally from high-level performance monitoring to detailed operational analysis.

---

# Assumptions and Limitations

## Assumptions

* All source data is accurate and complete.
* Return information correctly reflects completed product returns.
* Current Year and Previous Year calculations are based on available transaction dates.
* Profit calculations exclude external operational costs not present in the dataset.

## Limitations

* Customer lifetime value was not available.
* Inventory availability was not included in the dataset.
* Marketing campaign performance was limited to available campaign information.
* External business factors such as seasonality, competitor activity, and economic conditions were not considered.

---

# Tools Used

* Tableau Desktop
* Microsoft Excel
* Markdown Documentation

---

# Repository Structure

```
part4_tableau_dashboard/
│
├── data/
│   └── dashboard_sales_data.xlsx
│
├── tableau/
│   └── executive_dashboard.twbx
│
├── outputs/
│   ├── business_insights.md
│   ├── dashboard_story.md
│   └── chart_selection_justification.md
│
├── screenshots/
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   ├── filter_interaction_view.png
│   └── kpi_cards.png
│
└── README.md
```

---

# Screenshots Included

The repository includes the following screenshots as evidence of dashboard development:

* Full Executive Dashboard
* Sales Trend View
* Regional Performance View
* Category Profitability View
* Filter Interaction View
* KPI Cards

---

# Conclusion

The Retail Executive Performance Dashboard provides a comprehensive, interactive, and executive-friendly view of retail business performance.

By integrating KPIs, trend analysis, regional insights, customer analysis, profitability, shipping performance, discount effectiveness, and return analysis into a single dashboard, the solution enables leadership to make faster, evidence-based business decisions while supporting continuous performance monitoring.
