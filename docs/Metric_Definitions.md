# RetailMax | Metric Definitions and Review Status

The following are the definitions to confirm in the original model. They are not a reconstruction of the original DAX. The PDF cannot reveal calculation logic, relationships, filter context or row-level data.

| Metric | Definition to establish | Review status |
| --- | --- | --- |
| Revenue | Sum of the agreed sales amount at the documented transaction grain, with explicit treatment of discounts, tax, returns and cancellations. | Export shows £112.08M; underlying calculation has not been reconciled. |
| Gross profit | Revenue less the corresponding product costs under the same filters. | Export shows £27.87M; confirm cost and revenue use the same basis. |
| Gross margin | Gross profit divided by revenue, using consistent populations. | Export shows 24.87%. The rounded totals imply about 24.87%, which is a display-level check only. |
| Transactions | Distinct valid transaction IDs at the documented grain. Establish whether one ID is an order or an order line. | Executive card shows 50K; product card shows 275K. Reconciliation is needed. |
| Units sold | Sum of valid quantities, with a documented rule for returns and adjustments. | A possible explanation for the 275K card; this has not been verified. |
| Average transaction value | Revenue divided by qualifying distinct transactions. | Executive card shows £2.24K; do not infer an exact denominator from rounded values. |
| Revenue per unit | Revenue divided by qualifying units. | Product page shows £407.38; confirm the quantity denominator and filters. |
| Customers | Distinct valid customer IDs for the stated population. Distinguish registered customers from purchasing customers. | Export displays 5K, rounded. |
| Repeat customers | Distinct customers with at least two qualifying purchases in a clearly stated observation window. | Repeat rate shows 99.94%; source logic and denominator need validation. |
| Customer retention | Customers from a defined earlier-period cohort who also purchase in the later period, divided by that earlier cohort. | Export shows 99.05%; period, cohort and status treatment are not established. |
| Average customer value | Revenue per qualifying customer over a specified period. | Export shows £22.20K. It must not be labelled predicted lifetime value without a separate lifetime-value model. |
| Average discount | The agreed row, quantity-weighted or revenue-weighted discount calculation. | Export shows 20.09%; weighting is not known. |
| Discounted revenue and profit | Explicitly define whether these are net-of-discount amounts or totals restricted to discounted transactions. | Export shows £110.37M and £27.18M; interpretation requires the original measures. |
| Year-on-year growth | Like-for-like revenue change compared with the corresponding prior-year period. | Export shows 49.95%; the year selection and date-model behaviour need validation. |
| Revenue contribution | Revenue in the selected group divided by an explicitly defined comparison total. | Product-page card shows 100.00%; confirm denominator and filter behaviour. |

## Evidence available in this release

- Four original report pages as PDF and PNG.
- Visible KPI values, chart labels and relative category/channel rankings.
- Supporting descriptive analysis and documented validation questions.

## Evidence needed for calculation validation

- The original Power BI `.pbix` file and its DAX measures.
- Source tables, their grain and key definitions.
- Relationships, date table and filter propagation rules.
- Revenue, discount, return and cancellation business rules.

The available export supports a portfolio explanation of the reporting work. It cannot independently establish source-data accuracy or calculation correctness.
