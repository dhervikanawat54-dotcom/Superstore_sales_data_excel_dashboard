# Superstore Sales Dashboard

## Description

The **Superstore Sales Dashboard** is an interactive Excel reporting solution built from transaction-level retail order data. Each row represents an order line and records the order, customer, shipping, location, product, sales, quantity, discount, and profit details. The dashboard converts this detailed data into a concise management view, helping users understand sales performance, profitability, order volume, and customer activity at a glance.

The layout uses summary KPI cards, pivot charts, and slicers. Users can filter results by **year**, **category**, and **region**, then compare performance across product categories, sub-categories, geographic regions, and customer segments. It is intended for sales managers, business analysts, and decision-makers who need quick, interactive retail insights without reviewing every individual record.

## Dashboard Highlights

- **Total Customers:** 1,297
- **Total Profit:** $286,397.02
- **Total Orders:** 9,994
- **Total Quantity:** 37,987
- Sales distribution by category
- Sales and profit comparison by sub-category
- Sales and profit by region
- Sales by segment
- Interactive filters for year, category, and region

## Key Visuals

| Visual | Purpose |
| --- | --- |
| KPI cards | Summarize customers, profit, orders, and quantity. |
| Sales by category | Shows the relative contribution of each product category. |
| Sales and profit by sub-category | Highlights high- and low-performing product lines. |
| Sales and profit by region | Compares commercial performance across geographic regions. |
| Sales by segment | Shows how revenue is distributed among customer segments. |
| Slicers | Filter the entire dashboard by year, category, and region. |

## How to Use

1. Open the Excel workbook containing the dashboard.
2. Use the slicers on the left to select one or more years, categories, or regions.
3. Review the KPI cards for the filtered totals.
4. Use the charts to compare product, regional, and customer-segment performance.
5. Clear slicer selections to return to the full data view.

## Source Data

The source is a Superstore-style transactional sales table. A single order may appear in multiple rows because each row represents a different product line. For example, order `CA-2011-115812` contains several items across Furniture, Office Supplies, and Technology.

| Data Area | Fields |
| --- | --- |
| Order and shipping | Row ID, Order ID, Order Date, Ship Date, Ship Mode |
| Customer | Customer ID, Customer Name, Segment |
| Location | Country, City, State, Postal Code, Region |
| Product | Product ID, Category, Sub-Category, Product Name |
| Measures | Sales, Quantity, Discount, Profit |

### Data Notes

- Dates are stored in `DD-MM-YYYY` format and support the year slicer.
- **Sales**, **Profit**, and **Discount** should be numeric fields.
- Profit may be negative, indicating an unprofitable line item.
- **Order ID** is not unique at row level; count distinct Order IDs for total orders.
- Count distinct Customer IDs for total customers.
- Refresh PivotTables and PivotCharts after adding new data rows.

## Metric Definitions

| Metric | Calculation |
| --- | --- |
| Total Customers | Distinct count of `Customer ID` |
| Total Profit | Sum of `Profit` |
| Total Orders | Distinct count of `Order ID` |
| Total Quantity | Sum of `Quantity` |
| Category sales | Sum of `Sales`, grouped by `Category` |
| Sub-category performance | Sum of `Sales` and `Profit`, grouped by `Sub-Category` |
| Regional performance | Sum of `Sales` and `Profit`, grouped by `Region` |
| Segment sales | Sum of `Sales`, grouped by `Segment` |

## Dashboard Screenshot

##if you like this project

please consider it and give it a **star

##Author

**Dhanlaxmi kanawat**
_ _ _

![Superstore Sales Dashboard](C:/Users/hp/OneDrive/Pictures/Screenshots/Screenshot%202026-09-04%20171635.png)
