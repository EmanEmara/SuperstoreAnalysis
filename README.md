# Superstore Sales Dashboard (Excel)

An interactive Excel dashboard that analyzes four years of US retail sales from the Superstore dataset. It uses PivotTables, charts and slicers, with no macros or add-ins.

## Overview

The workbook turns 9,800 order lines into a one-page dashboard. You can see how sales change over time and which products, regions, customer segments and shipping methods drive them. The slicers filter every chart at once.

| | |
|---|---|
| **Period** | Jan 2015 – Dec 2018 |
| **Order lines** | 9,800 (4,922 unique orders) |
| **Customers / Products** | 793 / 1,861 |
| **Geography** | 49 US states, 4 regions |
| **Total sales** | ≈ $2.26M |

## Workbook structure

| Sheet | Purpose |
|---|---|
| `Dashboard` | The finished view: 7 charts and slicers |
| `PivotTables` | The 7 PivotTables (and their charts) that feed the dashboard |
| `StoreSales` | Raw data: 9,800 rows × 18 columns, with named ranges for each column |
| `Sheet4` | Scratch sheet used to count distinct products |

## Dashboard charts

1. **Sales by Sub-Category** (bar)
2. **Sales Over Time** (line)
3. **Growth Over Years** (line)
4. **Sales by Category** (pie)
5. **Segment Growth** (line)
6. **Shipping Mode Across Orders** (pie)
7. **Sales by Region** (bar)

**Slicers:** Years (Order Date), Segment, Ship Mode.

## Data dictionary (`StoreSales`)

| Column | Description |
|---|---|
| Row ID | Unique row number |
| Order ID | Order identifier (an order can have several lines) |
| Order Date / Ship Date | Dates the order was placed and shipped |
| Ship Mode | Standard Class, Second Class, First Class, Same Day |
| Customer ID / Customer Name | Customer identifiers |
| Segment | Consumer, Corporate, Home Office |
| Country / City / State / Postal Code / Region | Delivery location (Region: West, East, Central, South) |
| Product ID | Product identifier |
| Category / Sub-Category | Furniture, Office Supplies, Technology, and their sub-categories |
| Product Name | Product description |
| Sales | Sales amount in USD for the order line |

## Key figures

- **Sales by category:** Technology is highest (~$827K), then Furniture (~$729K) and Office Supplies (~$705K). Office Supplies has the most order lines (5,909).
- **Sales by region:** West leads (~$710K), followed by East, Central and South.
- **Sales by year:** 2015 ~$480K, 2016 ~$459K, 2017 ~$600K, 2018 ~$722K.
- **Top sub-categories:** Phones, Chairs and Storage.
- **Shipping:** Standard Class handles about 60% of order lines.

## How to use

1. Download `superstore.xlsx` and open it in Microsoft Excel. Slicers and PivotTables need desktop Excel 2013 or later. They may not work in Google Sheets or LibreOffice.
2. Open the **Dashboard** sheet.
3. Click the slicers to filter by year, segment or ship mode. All charts update together.
4. To refresh after changing the data, use **Data → Refresh All**.

## Skills demonstrated

Data cleaning and preparation, PivotTables, PivotCharts, slicers, named ranges, dashboard layout and sales trend analysis.





