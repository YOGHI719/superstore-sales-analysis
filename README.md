# Superstore Sales Analysis — SQL, Excel & Power BI

## Overview
End-to-end analysis of 150 retail orders across 4 regions, 4 product categories, and 6 sales representatives. The goal was to answer real business questions a regional manager would ask, using three tools together: SQL for querying, Excel for validation and quick summaries, and Power BI for an interactive dashboard.

**Dataset:** 150 orders | 14 columns (OrderID, OrderDate, Region, City, Category, Product, Segment, SalesRep, ShipMode, Quantity, UnitPrice, Discount, Sales, Profit)

## Tools Used
- **SQL (SQLite)** — data querying and business-question analysis
- **Excel** — Pivot Tables, SUMIFS/COUNTIFS/AVERAGEIFS
- **Power BI** — interactive dashboard with cross-filtering

## Key Business Questions Answered
1. Which region generates the most revenue and profit?
2. Which product category is most profitable?
3. Who are the top-performing sales reps?
4. Which orders resulted in a loss, and why?
5. How does discounting vary by region?
6. What is the monthly sales trend across the year?
7. How is the customer base split across segments?

## Key Findings

**1. Regional Performance**
West region leads in revenue (₹2.2M), but South leads in profit (₹407.9K) despite lower sales — indicating West may be over-discounting or selling lower-margin products relative to South.

**2. Category Profitability**
Electronics is the clear profit driver (₹775K), more than double the next category (Furniture, ₹338K). Clothing and Stationery contribute comparatively little profit despite reasonable order volume — worth reviewing their pricing or discount strategy.

**3. Sales Rep Performance**
Vikram is the top performer (₹1.84M in sales), nearly double the lowest performer, Anita (₹0.88M). This gap may point to a coaching or account-distribution opportunity.

**4. Loss-Making Orders**
A small number of orders were sold at a loss, several tied to high discount rates (15–20%). One order in particular resulted in a loss of over ₹15,000 — flagged as an outlier worth investigating (possible pricing error or excessive discount approval).

**5. Customer Segments**
The customer base is reasonably balanced: Corporate (36%), Consumer (32%), Home Office (32%) — no single segment dominates, which reduces business risk from over-reliance on one customer type.

**6. Seasonality**
Sales dipped in February and April, then peaked strongly in August — useful for planning inventory and marketing spend around seasonal demand.

## Methodology
1. **SQL** — Wrote 8+ queries covering filtering, aggregation (GROUP BY, SUM/COUNT/AVG), multi-condition filtering (HAVING), and row-level categorization (CASE WHEN) to answer each business question directly against the raw data.
2. **Excel** — Rebuilt the key summaries as Pivot Tables and cross-validated the SQL results using SUMIFS/COUNTIFS/AVERAGEIFS formulas.
3. **Power BI** — Imported the dataset, built a relationship model, and created a 5-visual interactive dashboard (regional sales, category profit, monthly trend, sales rep performance, segment split) with cross-filtering enabled.

## Dashboard Preview
![Dashboard Screenshot](Screenshot%202026-09-23%20224204.png)
## Recommendations
- Investigate discounting policy in the West region to protect margins.
- Review pricing/promotion strategy for Clothing and Stationery categories.
- Pair lower-performing reps with top performers for coaching.
- Audit high-discount orders that resulted in losses before approval in future.
- Plan Q3 (August) inventory and staffing ahead of the seasonal peak.

---
*Project built as part of a self-directed Data Analyst upskilling plan — SQL, Excel, and Power BI applied together on a single dataset to mirror a real analyst workflow.*# superstore-sales-analysis
End-to-end sales analysis using SQL, Excel &amp; Power BI — regional performance, profit analysis, and interactive dashboard.
