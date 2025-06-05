# E-commerce-Sales-Performance-Report

![excel-to-powerbi-animated-diagram](Data_csv/MicrosoftPower.gif)


# 🛍️ Project: E-commerce Sales Performance Dashboard
## 🎯 Objective
- **What is the key pain point?**  
  The Sales and Business team wants to monitor and understand the overall sales performance of the online store, including which products and categories are generating the most revenue, and whether monthly sales targets are being met.
- **What is the ideal solution?**  
  A Power BI dashboard that provides:
  -Total revenue
  - Number of orders
  -Average order value
  -Top-selling products
  -Performance vs sales targets
  This dashboard will help decision-makers optimize stock, marketing focus, and set realistic sales goals.
## 👤 User Story
As a **Sales Manager**, I want a dashboard that summarizes the sales performance of the store.  
The dashboard should allow me to:
- Monitor KPIs such as total sales, orders, and top customers.
- Identify the best-selling products and categories.
- Compare actual sales to monthly targets.
- Analyze trends to improve future sales strategies.
With this data, I can make better decisions to improve product offerings and align team efforts with business goals

## 📊 Data Source

- **What data is needed to achieve our objective?**
We need data that includes:
- `Orders.csv`: contains order ID, customer ID, date of purchase, etc.
- `Order_Details.csv`: includes product names, quantities sold, and unit prices.
- `Sales_Target.csv`: monthly sales targets by category or overall.

---

## 🧰 Tools Used

- Power BI (for dashboard creation and interactivity)
- Power Query (for data cleaning and transformation)
- DAX (for KPI calculations)
- Excel / CSV files (as data source)

---

## 📈 Metrics & Visuals

The dashboard includes:
- 📌 **KPI Cards**:
  - Total Sales
  - Total Orders
  - Average Order Value

- 📊 **Visuals**:
  - Line Chart: Monthly Sales Trends
  - Bar Chart: Top 10 Selling Products
  - Pie / Donut Chart: Sales by Category
  - Matrix: Sales vs Target
  - Filters: Category, Country, Date

- 🔍 **Key Measures** (sample DAX):
```dax
Total Sales = SUMX('Order_Details', 'Order_Details'[Quantity] * 'Order_Details'[Unit Price])
Total Quantity = SUM('Order_Details'[Quantity])
Average Order Value = [Total Sales] / DISTINCTCOUNT('Orders'[Order ID])
```
#Design
## 📊 Dashboard Components Required
What should the dashboard contain based on the requirements provided?

To understand what it should contain, we need to figure out what questions the dashboard needs to answer:

What is the total revenue generated?

How many orders have been placed?

What is the average order value?

Which are the top 10 best-selling products?

What are the monthly sales trends?

Which product categories are contributing the most to total sales?

Are we meeting our monthly sales targets?

Who are the top customers by spending?

These questions will help sales managers and business decision-makers monitor performance, identify strengths and weaknesses, and adjust strategies accordingly.

## 🧪 Dashboard Mockup
What should it look like?

Some of the data visuals that may be appropriate for answering these questions include:

✅ Scorecards / KPI Cards

Total Sales

Total Orders

Average Order Value

📊 Bar Chart

Top 10 Selling Products

📈 Line Chart

Monthly Sales Trend

🧱 Treemap

Sales by Product Category

🧮 Matrix Table

Sales vs Target (by Month or Category)

📋 Table

Top Customers (Name, # of Orders, Total Spend)

🎯 Slicers (Filters)

By Date, Category, Country, or Customer Segment
