# Excel KPI Formula Reference

Use structured table references where possible and adjust names to match the workbook.

| KPI | Example formula | Check |
|---|---|---|
| Total Sales | `=SUM(SalesData[Sales])` | Confirm sales column excludes headers and contains numeric values |
| Total Profit | `=SUM(SalesData[Profit])` | Confirm profit definition and negative values |
| Achievement % | `=IFERROR(ActualSales/TargetSales,0)` | Prefer N/A instead of 0 if zero target means not applicable |
| Sales Variance | `=ActualSales-TargetSales` | Positive means above target |
| Profit Margin % | `=IFERROR(TotalProfit/TotalSales,0)` | Format as percentage; confirm sales is non-zero |
| Return Rate % | `=IFERROR(ReturnedOrders/EligibleOrders,0)` | Ensure numerator and denominator use the same grain |

## Reporting checks

- Keep actuals and targets on the same date and category scope.
- Reconcile KPI cards to source totals.
- Refresh PivotTables before taking screenshots.
- Test slicers after refreshing data.
- Clearly label sample or synthetic data.

The formulas are examples; validate names, definitions, and denominator behavior against the actual workbook.