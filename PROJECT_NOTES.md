# Project Notes

## Project Objective

Build an interactive Power BI dashboard for analyzing AdventureWorks internet sales across products, customers, geography, and time.

The report was designed to answer questions such as:

- How much revenue and profit are being generated?
- Which product categories and individual products contribute most to performance?
- Which customer segments are most valuable?
- Which countries and sales territories generate the most revenue?
- How does current performance compare with the previous year?
- How is revenue accumulating year-to-date?

## Report Pages

### 1. Executive Overview

Primary KPIs:

- Revenue
- Profit
- Profit Margin
- Orders
- Quantity Sold
- Average Order Value
- Revenue YoY %

Main visuals:

- Revenue vs Previous Year
- Revenue YTD vs Previous Year
- CalendarYear slicer

### 2. Product Analysis

Primary KPIs:

- Profit Margin
- Profit
- Revenue
- Quantity Sold

Main visuals:

- Revenue by Product Hierarchy
- Top 10 Products by Profit
- Profit Margin by Category
- Top 10 Products by Quantity Sold

### 3. Customer Analysis

Primary KPIs:

- Customers
- Average Order Value
- Revenue
- Revenue per Customer

Main visuals:

- Revenue by Customer Occupation
- Customers by Income Group
- Revenue per Customer by Occupation
- Revenue by Income Group

### 4. Geographic Analysis

Primary KPIs:

- Revenue
- Profit
- Orders
- Quantity Sold

Main visuals:

- Revenue by Country
- Revenue by Region

### 5. Time Analysis

Primary KPIs:

- Revenue
- Revenue Previous Year
- Revenue YoY %

Main visuals:

- Revenue vs Previous Year
- Revenue YTD vs Previous Year
- Revenue YoY % by Month
- Revenue YTD YoY % by Month

## Semantic Model

The model is centered on `FactInternetSales` and connected to the following dimensions:

- `DimDate`
- `DimCustomer`
- `DimProduct`
- `DimProductSubcategory`
- `DimProductCategory`
- `DimSalesTerritory`

The model supports drill-down from product category to subcategory and product, while customer, date, and territory dimensions provide analytical slicing.

## Measures Used

Business measures visible in the report include:

| Measure | Purpose |
|---|---|
| Revenue | Total sales revenue |
| Cost | Total product cost |
| Profit | Revenue after cost |
| Profit Margin | Profit as a percentage of revenue |
| Orders | Number of orders |
| Quantity Sold | Units sold |
| Customers | Distinct customers |
| Average Order Value | Revenue per order |
| Revenue per Customer | Revenue divided by customers |
| Revenue Previous Year | Comparable revenue from the prior year |
| Revenue YoY % | Year-over-year revenue growth |
| Revenue YTD | Cumulative revenue within the selected year |
| Revenue YTD Previous Year | Previous-year cumulative revenue |
| Revenue YTD YoY % | YTD growth versus previous year |

## Selected 2013 Results

- Revenue: **$16.35M**
- Profit: **$6.77M**
- Profit Margin: **41.37%**
- Orders: **21K**
- Quantity Sold: **53K**
- Average Order Value: **$768.08**
- Revenue Previous Year: **$5.84M**
- Revenue YoY: **179.87%**
- Customers: **17K**
- Revenue per Customer: **$938.18**

## Analytical Findings

### Products

Bikes account for the overwhelming majority of revenue. Accessories and Clothing contribute much less revenue, but Accessories show the strongest margin percentage.

The highest-profit products are concentrated among Mountain-200 bike variants. In unit volume, smaller accessories such as the Water Bottle - 30 oz. and Patch Kit/8 Patches rank among the strongest sellers.

### Customers

Professional customers generate the most revenue. The Professional and Management groups also lead on revenue per customer.

The 60K income segment is the largest by customer count and revenue.

### Geography

The United States leads country-level revenue, followed by Australia. At the sales-region level, Australia and Southwest are the strongest performers in the selected view.

### Time

Current-year revenue is above previous-year revenue across the months shown. Monthly YoY growth peaks around May, while February is the lowest-growth month. Cumulative YTD revenue continues to widen its lead over the previous year through December.

## Design Approach

The report uses:

- Light-gray page backgrounds
- White visual containers
- A consistent blue accent
- Compact KPI cards
- Consistent spacing and alignment
- Short, business-readable chart titles
- Calendar-year slicers for interactive filtering
