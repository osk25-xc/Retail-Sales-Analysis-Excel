# Retail Sales Excel Workbook QA Checklist

Use this after refreshing the source data and before sharing the workbook.

## Source and refresh
- [ ] Confirm the source range is an Excel Table or otherwise expands to include new rows.
- [ ] Refresh queries and PivotTables; check refresh errors.
- [ ] Verify dates, quantities, sales, cost, and order identifiers use suitable data types.
- [ ] Review blanks, duplicate keys, and invalid values.

## KPI reconciliation
- [ ] Reconcile total sales and profit to the source records.
- [ ] Calculate profit margin from aggregate profit divided by aggregate sales.
- [ ] Count distinct orders rather than line-item rows when the source is at line-item grain.
- [ ] Document the denominator for delivery and return rates.

## PivotTable and slicer tests
- [ ] Confirm PivotTable fields and aggregation methods are correct.
- [ ] Test every slicer and report filter.
- [ ] Confirm relevant KPI cards, PivotCharts, and summaries respond to filters.
- [ ] Check that clearing filters restores the expected overall totals.

## Sign-off
- [ ] Record the refresh date, filters, exclusions, and known limitations.
- [ ] Capture screenshots only from the verified workbook.
- [ ] Do not claim an interaction works until it has been tested in Excel.