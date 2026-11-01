# Retail Sales Excel Dashboard — KPI Definitions

The workbook and accompanying practice dataset use the following field names.

| KPI | Calculation | Reporting note |
|---|---|---|
| Total Sales | Sum of `Sales` | Use the active slicer/filter context |
| Total Profit | Sum of `Profit` | Use the same filtered records as sales |
| Profit Margin % | Total Profit / Total Sales × 100 | Calculate from aggregated totals, not by averaging row percentages |
| Order Count | Distinct count of `Order ID` | Avoid counting duplicate order IDs as separate orders |
| Units Sold | Sum of `Quantity` | Confirm whether cancelled orders are included in the source |

## Dataset fields

`Order ID`, `Order Date`, `Region`, `Category`, `Product`, `Quantity`, `Unit Price`, `Sales`, `Cost`, and `Profit`.

## Validation checks

- Check that `Sales` is consistent with `Quantity × Unit Price` where that is the dataset rule.
- Check that `Profit` is consistent with `Sales − Cost`.
- Confirm that order IDs are counted distinctly.
- Reconcile category and region totals to the grand total.
- Test each KPI with the Region slicer to confirm the displayed values respond to filters.
- Refresh PivotTables after replacing or updating the source data.

## Interpretation

Profit margin is a ratio of aggregated profit to aggregated sales. A region with the highest sales does not necessarily have the highest profit margin. The dataset is for portfolio practice and should not be presented as actual company performance.
