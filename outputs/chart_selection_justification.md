# Chart Selection Justification

## Overview

The dashboard was designed using visualization best practices to ensure that each chart answers a specific business question. Chart selection was based on the nature of the data, the analytical objective, and executive usability rather than visual appearance. Interactive features such as global filters, parameter actions, dashboard actions, and Viz in Tooltip were incorporated to enhance exploratory analysis while maintaining a clean and uncluttered layout.

---

# 1. Executive KPI Cards

## Business Question

How is the business performing overall?

## Chart Selected

Executive KPI Cards

## Reason for Selection

KPI cards provide an immediate summary of the most important business metrics without requiring users to interpret charts. Executives can quickly monitor overall performance and compare current performance against the previous year.

## Measures Used

* Total Sales
* Total Profit
* Total Orders
* Return Rate

Each KPI includes:

* Current Year Value
* Previous Year Value
* Year-over-Year Growth %
* Performance Indicator (▲ / ▼)

## Design Principles Applied

* Large typography for immediate visibility
* Consistent color palette across all KPIs
* Conditional formatting for growth indicators
* Minimal visual clutter

## Visualization Alternative Avoided

Pie charts or gauges were avoided because they consume more space and communicate KPI values less efficiently than summary cards.

---

# 2. Sales Trend Analysis

## Business Question

How has business performance changed over time?

## Chart Selected

Line Chart

## Reason for Selection

A line chart is the most appropriate visualization for displaying trends across time. It enables users to quickly identify seasonal patterns, growth, declines, and performance fluctuations.

Instead of creating separate charts for Sales, Profit, and Orders, a parameter-driven design allows users to dynamically switch between the three metrics within a single visualization.

## Fields Used

* X-axis: Order Month
* Y-axis: Selected Metric (Sales, Profit, or Orders)

## Interactive Features

* Parameter Action
* Dynamic metric switching

## Design Principles Applied

* Consistent monthly timeline
* Clear data labels
* Minimal gridlines
* Easy comparison across months

## Visualization Alternative Avoided

Bar charts were avoided because they require more visual space and are less effective for displaying continuous trends.

---

# 3. Regional Performance

## Business Question

Which regions contribute the most sales?

## Chart Selected

Horizontal Bar Chart

## Reason for Selection

Horizontal bar charts provide the clearest comparison between categorical values and allow region names to remain fully readable.

The visualization is sorted in descending order to immediately identify the highest-performing regions.

## Fields Used

* Dimension: Region
* Measure: Sales

## Interactive Features

Viz in Tooltip displays additional sales breakdown by State and City.

## Design Principles Applied

* Descending sorting
* Consistent color palette
* Readable labels
* Rich tooltip for drill-down analysis

## Visualization Alternative Avoided

Maps were avoided because the objective was comparison rather than geographical location. Horizontal bars provide more accurate visual comparison.

---

# 4. Category Profitability

## Business Question

Which product categories generate the highest profit?

## Chart Selected

Horizontal Bar Chart

## Reason for Selection

The chart enables quick ranking of product sub-categories based on profitability. Sorting and color intensity help users identify both strong and weak performing products.

## Fields Used

* Dimension: Sub-Category
* Measure: Profit

## Design Principles Applied

* Descending ranking
* Color intensity based on profit
* Minimal chart clutter

## Visualization Alternative Avoided

Treemaps were considered but rejected because they make precise comparison between product categories more difficult.

---

# 5. Shipping Performance

## Business Question

How efficiently are customer orders being delivered?

## Charts Selected

* Horizontal Bar Chart (Average Delivery Days)
* Horizontal Bar Chart (Order Distribution)

## Reason for Selection

Using two complementary bar charts allows executives to simultaneously evaluate shipping speed and the proportion of orders within each delivery bucket.

This combination provides more operational insight than a single chart.

## Fields Used

* Shipping Delay Bucket
* Average Shipping Days
* Percentage of Orders

## Design Principles Applied

* Consistent axis
* Simple categorical comparison
* Executive-friendly labels

## Visualization Alternative Avoided

Pie charts were avoided because they make comparison between delivery categories less accurate.

---

# 6. Customer Segment Performance

## Business Question

How do different customer segments compare?

## Chart Selected

Performance Scorecard (Highlight Table with In-cell Bars)

## Reason for Selection

Instead of using another bar chart, a compact scorecard allows multiple KPIs to be compared simultaneously for each customer segment.

The design displays:

* Sales
* Profit Margin
* Average Order Value (AOV)

within a single visualization.

## Fields Used

* Customer Segment
* Sales
* Profit Margin
* Average Order Value

## Design Principles Applied

* Compact layout
* In-cell data bars
* Easy side-by-side comparison
* Reduced dashboard space

## Visualization Alternative Avoided

Dual-axis charts and clustered bar charts were avoided because they introduce unnecessary complexity and consume more dashboard space.

---

# 7. Discount Impact on Profitability

## Business Question

How do discounts influence profitability?

## Chart Selected

Scatter Plot

## Reason for Selection

A scatter plot is the most appropriate visualization for identifying relationships between two continuous numerical variables.

Each mark represents an individual order, allowing users to identify profitable and loss-making transactions at different discount levels.

Reference lines divide the chart into analytical quadrants for easier interpretation.

## Fields Used

* X-axis: Average Discount
* Y-axis: Profit
* Detail: Order ID
* Color: Profit / Loss

## Design Principles Applied

* Reference lines
* Color encoding
* Minimal overlap
* Executive interpretation

## Visualization Alternative Avoided

Line charts and bar charts were avoided because they cannot effectively display relationships between two continuous variables.

---

# 8. Return Hotspots

## Business Question

Which product categories experience the highest return rates?

## Chart Selected

Heatmap

## Reason for Selection

A heatmap enables executives to quickly identify return hotspots using color intensity without requiring detailed numerical analysis.

The hierarchical layout (Category → Sub-Category) provides both summary and detailed insights.

## Fields Used

* Category
* Sub-Category
* Return Rate

## Interactive Features

Viz in Tooltip displays:

* Sales
* Profit
* Return Count
* Customer Segment breakdown

## Design Principles Applied

* Sequential color scale
* Hierarchical grouping
* Rich tooltip
* Efficient space utilization

## Visualization Alternative Avoided

Stacked bar charts were avoided because they require more space and make identifying return hotspots less intuitive.

---

# Dashboard-Level Interactive Features

Several advanced Tableau features were incorporated to improve usability and support interactive analysis.

## Global Filters

The dashboard includes filters for:

* Order Date
* Region
* Category
* Sub-Category
* Ship Mode
* Campaign Channel

All worksheets update simultaneously based on filter selections.

---

## Parameter Action

A parameter-driven metric selector allows users to dynamically switch the trend chart between:

* Sales
* Profit
* Orders

This improves dashboard usability while avoiding duplicate visualizations.

---

## Dashboard Actions

Interactive filter actions enable users to select a region or data point and instantly update related visualizations, encouraging deeper exploration of the data.

---

## Viz in Tooltip

Embedded visualizations inside tooltips provide additional contextual analysis without increasing dashboard complexity.

This feature has been implemented for:

* Regional Performance
* Return Hotspots

---

## Reset Filters

A dedicated Reset Filters button allows users to quickly restore the dashboard to its default state after interactive exploration.

---

# Visualization Design Principles Applied

The following visualization principles guided the dashboard design:

* Appropriate chart selection based on business questions.
* Consistent color palette throughout the dashboard.
* Clear visual hierarchy using KPI cards and section titles.
* Minimal clutter with sufficient white space.
* Consistent formatting and typography.
* Descending sorting where comparison is required.
* Interactive exploration through filters and actions.
* Executive-friendly layout emphasizing readability over decoration.

---

# Conclusion

Each visualization in the dashboard was selected based on its ability to answer a specific business question while supporting executive decision-making.

The combination of KPI cards, line charts, bar charts, scorecards, scatter plots, heatmaps, and advanced Tableau interactions creates a comprehensive and user-friendly analytical dashboard that enables leadership to monitor performance, identify risks, and uncover business opportunities efficiently.
