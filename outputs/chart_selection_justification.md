# Chart Selection Justification

## 1. Monthly Sales Trend

### Business Question
How do sales change over time?

### Chart Type
Line Chart

### Why This Chart?
A line chart is the most appropriate visualization for displaying trends over time. It allows management to quickly identify seasonal patterns, monthly fluctuations, and long-term sales performance.

### Fields Used
- X-axis: Order Date (Month)
- Y-axis: SUM(Sales)

### Design Principles Applied
- Chronological order maintained.
- Simple blue color scheme for readability.
- Clear title and axis labels.
- Minimal visual clutter.

### Mistakes Avoided
- Avoided using bar charts, which make continuous time trends harder to interpret.
- Avoided unnecessary colors that could distract from the trend.

---

## 2. Regional Sales & Profit Performance

### Business Question
Which region contributes the most sales?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A horizontal bar chart makes it easy to compare sales across regions. Sorting the bars highlights the highest and lowest performing regions immediately.

### Fields Used
- Rows: Region
- Columns: SUM(Sales)
- Color: SUM(Profit)

### Design Principles Applied
- Bars sorted from highest to lowest.
- Profit represented using color intensity.
- Data labels displayed for quick comparison.

### Mistakes Avoided
- Avoided pie charts, which make comparing similar values difficult.
- Avoided unnecessary 3D effects.

---

## 3. Category Profitability

### Business Question
Which product categories and sub-categories generate the most profit?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A horizontal bar chart provides a clear comparison of profitability across multiple product categories and sub-categories, making it easy to identify top and bottom performers.

### Fields Used
- Rows: Sub-Category
- Columns: SUM(Profit)
- Color: Category

### Design Principles Applied
- Descending sort order.
- Consistent category colors.
- Profit values shown as labels.

### Mistakes Avoided
- Avoided stacked charts that would reduce readability.
- Avoided excessive colors that could confuse category comparisons.

---

## 4. Customer Segment Performance

### Business Question
Which customer segment generates the highest sales?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A bar chart clearly compares sales across customer segments and allows management to identify the most valuable customer groups.

### Fields Used
- Rows: Customer Segment
- Columns: SUM(Sales)
- Color: Customer Segment

### Design Principles Applied
- Clear labels.
- Consistent spacing.
- Sorted values for easier comparison.

### Mistakes Avoided
- Avoided pie charts because differences between segments are easier to compare using bars.

---

## 5. Discount vs Profit

### Business Question
How do discounts affect profitability?

### Chart Type
Scatter Plot with Trend Line

### Why This Chart?
A scatter plot is the best choice for showing the relationship between two continuous variables. The trend line highlights the overall relationship between discount percentage and profit.

### Fields Used
- X-axis: Discount
- Y-axis: Profit
- Color: Category
- Trend Line: Linear

### Design Principles Applied
- Semi-transparent circles reduce overlap.
- Trend line summarizes the overall relationship.
- Category colors improve interpretation.

### Mistakes Avoided
- Avoided line charts because discount values are not sequential time data.
- Avoided bar charts because they cannot effectively display correlations between two numeric variables.

---

# Dashboard Design Principles

The dashboard was designed to support executive decision-making by emphasizing clarity, simplicity, and business relevance.

The design follows these principles:

- Consistent color palette across all visualizations.
- Clear and descriptive chart titles.
- Appropriate chart selection based on the business question.
- Minimal visual clutter.
- Readable axis labels and data labels.
- Logical arrangement of charts.
- KPI cards positioned at the top for quick performance overview.
- Interactive Region filter allows users to explore regional performance efficiently.
- Consistent formatting across all dashboard components.

Overall, the dashboard enables management to quickly monitor business performance, compare key metrics, and identify areas requiring further investigation.
