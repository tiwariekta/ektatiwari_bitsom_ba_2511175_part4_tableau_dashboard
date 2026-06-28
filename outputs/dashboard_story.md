# Dashboard Story

## Retail Executive Performance Dashboard

---

# 1. Executive Summary

The **Retail Executive Performance Dashboard** is designed to provide business leaders with a consolidated view of retail performance across sales, profitability, customer behavior, shipping efficiency, and product returns.

Instead of analyzing multiple reports individually, executives can monitor key business metrics from a single interactive dashboard and quickly identify trends, operational bottlenecks, and areas requiring attention.

The dashboard enables users to:

* Monitor overall business performance through executive KPIs
* Compare sales and profitability across different regions
* Identify high-performing and low-performing product categories
* Evaluate customer segments based on sales and profitability
* Understand the impact of discounts on profitability
* Detect return hotspots at the product sub-category level
* Interactively explore data using global filters and drill-down tooltips

---

# 2. Executive KPI Overview

The dashboard begins with four executive KPI cards summarizing overall business performance.

### Total Sales

Displays the total sales generated during the selected period along with:

* Previous Year Sales
* Year-over-Year (YoY) Growth %
* Visual indicator showing positive or negative performance

### Total Profit

Shows the overall profit generated together with:

* Previous Year Profit
* YoY Growth %
* Performance indicator

### Total Orders

Displays the total number of customer orders processed.
Users can immediately compare current performance against the previous year.

### Return Rate

Measures the percentage of returned orders.

Unlike the other KPIs, lower return rates indicate better operational performance. Conditional formatting highlights increases in return rate using red indicators to draw executive attention.

---

# 3. Sales Trend Analysis

The Sales Trend section provides a month-over-month view of business performance.

Instead of creating multiple charts, a parameter-driven design allows executives to dynamically switch between:

* Sales
* Profit
* Orders

using simple metric selectors.

This interactive approach reduces dashboard clutter while allowing users to analyze different business metrics within the same visualization.

Data labels are displayed to improve readability and allow executives to quickly identify seasonal trends and monthly fluctuations.

---

# 4. Regional Performance

Regional Performance compares total sales across all business regions.

The horizontal bar chart enables easy comparison between regions and clearly identifies the strongest and weakest performing markets.

Additional interactivity has been implemented using **Viz in Tooltip**.

When users hover over a region, a detailed tooltip displays:

* Sales breakdown by State
* Sales contribution by City

This allows executives to drill down into regional performance without navigating away from the dashboard.

---

# 5. Category Profitability

This visualization ranks product sub-categories based on total profit.

The chart highlights:

* Highest profit generating product categories
* Lower profit categories requiring attention

Positive performers are emphasized using darker green shades while lower-profit categories are shown using lighter colors to improve visual interpretation.

The ranking helps identify which product categories contribute most toward overall profitability.

---

# 6. Shipping Performance

Shipping performance is evaluated using two complementary metrics:

### Average Delivery Days

Displays the average number of days taken to deliver orders across predefined shipping delay buckets.

### Order Distribution

Shows the percentage of total orders falling within each shipping delay category.

Together, these metrics provide insight into logistics efficiency while helping identify operational bottlenecks affecting customer satisfaction.

---

# 7. Customer Segment Performance

Customer performance is summarized across the three customer segments:

* Consumer
* Corporate
* Home Office

For each segment the dashboard displays:

* Total Sales
* Profit Margin
* Average Order Value (AOV)

In-cell bars are used for Sales to allow quick visual comparison while maintaining a compact tabular layout suitable for executive reporting.

---

# 8. Discount Impact on Profitability

Understanding the relationship between discounting and profitability is essential for retail decision-making.

A scatter plot has been used to analyze the relationship between:

* Average Discount
* Profit

Additional analytical elements include:

* Average Discount reference line
* Average Profit reference line
* Green marks representing profitable orders
* Red marks representing loss-making orders

This visualization helps identify discount levels where profitability begins to decline and supports pricing strategy decisions.

---

# 9. Return Hotspots Analysis

Product returns directly impact profitability.

The Return Hotspots heatmap visualizes return rates across product categories and sub-categories using color intensity.

Darker shades indicate higher return rates, allowing executives to quickly identify problematic product groups.

Each heatmap cell includes a detailed tooltip displaying:

* Sales
* Profit
* Returned Orders
* Return Rate
* Customer Segment-wise performance

This enables deeper investigation into return behavior without leaving the dashboard.

---

# 10. Dashboard Interactivity

Several interactive Tableau features have been incorporated to improve usability and encourage data exploration.

### Global Filters

The dashboard includes global filters for:

* Order Date
* Region
* Category
* Sub-Category
* Ship Mode
* Campaign Channel

All visualizations respond dynamically to the selected filters.

### Parameter Actions

Users can switch the trend visualization between Sales, Profit, and Orders using parameter-driven metric selection.

### Action Filters

Interactive dashboard actions allow users to explore related information across visualizations while maintaining analytical context.

### Viz in Tooltip

Regional Performance and Return Hotspots include embedded visualizations inside tooltips, enabling users to drill into additional details without opening separate worksheets.

### Reset Filters

A dedicated Reset Filters button restores the dashboard to its default state, improving user experience during exploratory analysis.

---

# 11. Key Business Recommendations

Based on the dashboard analysis, the following recommendations can help improve business performance:

* Review pricing strategies for products requiring heavy discounts to maintain profitability.
* Investigate sub-categories with consistently high return rates and identify potential product quality or fulfillment issues.
* Increase investment in highly profitable product categories while reviewing underperforming categories.
* Improve shipping performance for delayed orders to enhance customer satisfaction.
* Continue monitoring customer segment performance to optimize marketing and sales strategies.
* Focus regional sales initiatives in lower-performing markets while sustaining growth in high-performing regions.

---

# 12. Conclusion

The Retail Executive Performance Dashboard provides a comprehensive and interactive view of overall business performance.

By combining executive KPIs, trend analysis, profitability analysis, customer insights, logistics monitoring, and return analysis into a single dashboard, business users can make faster, data-driven decisions.

The use of interactive filters, parameter actions, drill-down tooltips, and dashboard actions creates a user-friendly analytical experience while enabling both high-level monitoring and detailed investigation.
