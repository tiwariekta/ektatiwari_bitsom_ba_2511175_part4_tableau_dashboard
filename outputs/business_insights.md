# Calculated Fields Used

The dashboard uses several calculated fields to provide year-over-year comparison, operational KPIs, and business performance metrics.

---

## 1. Previous Year (PY) Calculations

Previous Year metrics are calculated using Tableau's `DATEADD()` function by shifting the order date back one year.

Example:

```tableau
IF DATETRUNC('month',[Order Date])
=
DATEADD('year',1,DATETRUNC('month',[Order Date]))
```

These calculations provide the baseline required for Year-over-Year comparisons across Sales, Profit, Orders, and Return Rate.

Business Purpose:
- Enables annual performance comparison.
- Measures business growth over time.
- Supports executive KPI monitoring.

---

## 2. Year-over-Year Growth %

Growth percentage is calculated as:

(Current Year - Previous Year)
/ Previous Year

Business Purpose:
- Shows business growth instead of only absolute values.
- Allows quick identification of improving or declining performance.

Positive values are displayed in green, while negative values are highlighted in red.

---

## 3. Return Rate

Return Rate is calculated as:

Returned Orders
/
Total Orders

Business Purpose:
- Measures product return frequency.
- Helps identify operational or product quality issues.
- Supports return hotspot analysis.

---

## 4. Average Order Value (AOV)

Average Order Value is calculated as:

Sales
/
Number of Orders

Business Purpose:
- Measures average customer spending per order.
- Helps compare purchasing behaviour across customer segments.

---

## 5. Profit Margin

Profit Margin is calculated as:

Profit
/
Sales

Business Purpose:
- Evaluates profitability independent of revenue.
- Allows comparison across customer segments and product categories.

---

## 6. Delivery Delay Bucket

Shipping performance is grouped into four business-friendly categories.

Example:

- Fast (0–2 Days)
- Normal (3–5 Days)
- Delayed (6–7 Days)
- Highly Delayed (>7 Days)

Business Purpose:
- Simplifies shipment analysis.
- Helps management monitor logistics performance.

---

## 7. Average Discount Reference Line

Average Discount is calculated using:

AVG(Discount)

Business Purpose:
- Serves as a benchmark in the Discount vs Profit scatter plot.
- Helps identify heavily discounted orders.

---

## 8. Average Profit Reference Line

Average Profit is calculated using:

AVG(Profit)

Business Purpose:
- Separates above-average and below-average performing orders.
- Highlights potentially loss-making transactions.

---

## 9. Dynamic Trend Metric

A parameter allows users to switch between:

- Sales
- Profit
- Orders

The line chart automatically updates based on the selected metric.

Business Purpose:
- Reduces dashboard clutter.
- Allows multiple KPIs to be analysed within a single visualization.

---

## 10. KPI Cards

Each KPI card displays:

- Current Year Value
- Previous Year Value
- Percentage Change
- Direction Indicator (▲ / ▼)

Business Purpose:
- Provides executives with an immediate summary of overall business performance.


# Interactive Features

The dashboard incorporates several interactive features to improve exploratory analysis.

- Global filters update every worksheet simultaneously.
- A Reset Filters button restores the default dashboard state.
- Parameter-driven trend chart switches between Sales, Profit, and Orders.
- Regional tooltips provide city-level sales breakdowns.
- Return hotspot tooltips display customer-segment-wise return metrics.
- Hover tooltips provide additional business context without increasing dashboard complexity.

These interactive features enable executives to answer business questions with minimal navigation.
