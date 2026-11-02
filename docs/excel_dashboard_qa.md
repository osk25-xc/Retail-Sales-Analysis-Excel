# Excel Dashboard QA Checklist

## Source data
- Convert the source range to an Excel Table and confirm headers are unique.
- Check dates are real date values, not text.
- Identify duplicate order IDs separately from duplicate line items.
- Confirm numeric columns contain no text-formatted numbers or hidden errors.

## KPI reconciliation
- Total sales and profit should reconcile to source totals under the same filters.
- Profit margin should be total profit divided by total sales, not an average of row-level margins.
- Count orders with a distinct order ID where the data contains multiple lines per order.
- Confirm target achievement uses the agreed target denominator.

## Interactions
Test every slicer against every KPI card, PivotChart, and summary table. Refresh all PivotTables after source changes. Check month sorting across year boundaries.

## Evidence
Record the workbook version, refresh date, filter state, and reconciliation results before publishing screenshots or numerical claims.
