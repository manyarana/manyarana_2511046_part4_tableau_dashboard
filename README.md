# Retail Executive Dashboard using Tableau

## Business Problem

This project was developed to help a retail company's leadership team monitor overall business performance using an interactive Tableau dashboard. The objective is to provide a clear view of sales, profitability, customer segments, regional performance, and the impact of discounts so that business decisions can be made based on data rather than intuition.

---

# Dataset Description

The project uses the provided retail sales dataset (`dashboard_sales_data.xlsx`) containing transactional information, including:

- Order Date
- Ship Date
- Region
- State
- City
- Customer Segment
- Category
- Sub-Category
- Product Name
- Sales
- Profit
- Quantity
- Discount
- Delivery Days
- Return Flag
- Customer Rating
- Campaign Channel
- Ship Mode

The dataset includes both categorical and numerical fields suitable for business intelligence analysis.

---

# Tableau Workbook

The Tableau workbook (`executive_dashboard.twbx`) contains an interactive executive dashboard built for business leaders. It includes KPI cards, multiple visualizations, and interactive filters that allow users to explore business performance across different dimensions.

---

# Calculated Fields Created

The following calculated fields were created in Tableau:

## Profit Margin

```
SUM([Profit]) / SUM([Sales])
```

Calculates the percentage profit earned from total sales.

---

## Cost

```
SUM([Sales]) - SUM([Profit])
```

Calculates the estimated cost associated with sales.

---

## Average Order Value

```
SUM([Sales]) / COUNTD([Order ID])
```

Calculates the average sales value per order.

---

## Return Rate

```
SUM([Return Flag]) / COUNT([Order ID])
```

Calculates the percentage of returned orders.

---

## Shipping Delay Bucket

```
IF [Delivery Days] <= 2 THEN "Fast"
ELSEIF [Delivery Days] <= 5 THEN "Standard"
ELSE "Delayed"
END
```

Groups deliveries into meaningful shipping categories.

---

# Dashboard Components

The executive dashboard includes:

- KPI Card – Total Sales
- KPI Card – Total Profit
- KPI Card – Return Rate
- Monthly Sales Trend
- Regional Sales & Profit Performance
- Category Profitability
- Customer Segment Performance
- Discount vs Profit Analysis

---

# Filters and Interactions

The dashboard includes:

- Region Filter (applied to all dashboard charts)

Interactive filtering allows users to quickly compare performance across different regions.

---

# Key Business Insights

Some major findings from the dashboard include:

- Sales remain stable throughout the year.
- South is the highest-performing region.
- East and West have opportunities for growth.
- Technology products generate the highest profits.
- Larger discounts generally reduce profitability.
- Home Office customers contribute the highest sales.
- Overall return rate is low (4.55%).
- Strong sales performance provides opportunities for further profit optimization.

Detailed insights are available in:

`outputs/business_insights.md`

---

# Dashboard Story Summary

The dashboard tells a complete business story by combining sales trends, profitability, customer behavior, regional performance, and pricing analysis into a single executive view.

It helps management identify:

- Business strengths
- Weak-performing areas
- Financial risks
- Growth opportunities
- Recommended business actions

The complete narrative is available in:

`outputs/dashboard_story.md`

---

# Assumptions and Limitations

## Assumptions

- The provided dataset is accurate and complete.
- Sales and profit values are correctly recorded.
- Return Flag correctly identifies returned orders.
- Delivery Days accurately represent shipping performance.

## Limitations

- Historical data only; no predictive analysis.
- External factors such as competitors and economic conditions are not included.
- Customer demographics are not available.
- Marketing campaign effectiveness is outside the scope of this dashboard.

---

# Screenshots Included

The repository contains the following screenshots:

- `full_dashboard.png`
(https://github.com/manyarana/manyarana_2511046_part4_tableau_dashboard/blob/main/screenshots/full_dashboard.png)
- `sales_trend_view.png` (https://github.com/manyarana/manyarana_2511046_part4_tableau_dashboard/blob/main/screenshots/sales_trend_view.png)
- `regional_performance_view.png` (https://github.com/manyarana/manyarana_2511046_part4_tableau_dashboard/blob/main/screenshots/regional_performance_view.png)
- `category_profitability_view.png` (https://github.com/manyarana/manyarana_2511046_part4_tableau_dashboard/blob/main/screenshots/category_profitability_view.png)
- `filter_interaction_view.png` (https://github.com/manyarana/manyarana_2511046_part4_tableau_dashboard/blob/main/screenshots/filter_interaction_view.png)

These screenshots demonstrate the dashboard layout, individual visualizations, and interactive filtering.

---

# Repository Structure

```
part4_tableau_dashboard/
├── data/
│   └── dashboard_sales_data.xlsx
├── tableau/
│   └── executive_dashboard.twbx
├── outputs/
│   ├── business_insights.md
│   ├── dashboard_story.md
│   └── chart_selection_justification.md
├── screenshots/
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   └── filter_interaction_view.png
└── README.md
```

---

# Conclusion

This Tableau dashboard transforms raw retail sales data into an interactive executive reporting tool. By combining KPIs, visual analytics, and business storytelling, it enables leadership to monitor performance, identify opportunities, and make informed strategic decisions. The dashboard follows visualization best practices, supports interactive exploration, and presents business insights in a clear and accessible format.
