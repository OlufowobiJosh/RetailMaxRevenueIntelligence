# RetailMax | Data Quality Notes

This report-based release preserves the original export. The following issues are visible in the saved report and should be checked in the original model before the figures are used for business decisions.

| Check | Evidence in the export | Action in the source model |
| --- | --- | --- |
| Transaction count | Executive page: 50K. Product page: 275K. Both cards are titled "Total Transaction". | Check the measure assigned to each card, transaction grain, distinct-ID counts and page filters. Determine whether 275K represents units. Relabel it only after verification. |
| Repeat purchase and retention | Repeat Customer %: 99.94%. Customer Retention Rate %: 99.05%. | Verify distinct customers, qualifying orders, time windows, cohort membership and denominator. High values are not proof of an error, particularly in case-study data. |
| Blank dimension members | Several product, customer and loyalty charts show `(Blank)`. | Inspect missing attributes, unmatched foreign keys and dimension uniqueness. Use an explicit Unknown category only when the underlying cause is understood. |
| Revenue status policy | Completed, Returned and Cancelled each account for roughly one third of the displayed transaction split. | Establish whether headline revenue includes every status and how returns are signed. Do not present an all-status total as realised sales without the agreed policy. |
| Monthly and year-on-year analysis | Month names appear without a visible year selection; the executive card shows 49.95% YoY growth. | Check the date table, transaction-date relationship and comparable periods. Use year-month when multiple years are present. |
| Customer age bands | The report includes Under 18 and 91+ groups, with 91+ leading displayed age-group revenue. | Validate date of birth, age calculation, reference date, missing values and band sorting. Do not remove valid ages simply because they are unusual. |
| Geographic dimensions | Executive profit uses West/North/South/East; customer counts use labels such as North West and London. | Identify whether these refer to different concepts, such as trading region and home region. Label both clearly and document any mapping. |
| Discount interpretation | "Discounted Revenue", "Discounted Profit" and average discount appear without calculation definitions. | Establish subset versus net-value meaning and discount weighting. Do not claim a causal discount effect from the export. |
| Contribution card | Revenue Contribution % is 100.00% in the product-page overview. | Verify that the measure responds as intended when a category or channel is selected and uses the right comparison denominator. |

## Changes in this portfolio release

- Renamed the PDF for clarity without changing its bytes.
- Exported the four pages to PNG without changing charts or numbers.
- Added descriptive documentation and recorded the open metric questions.

No calculations, source rows or chart values were altered. Re-export the PDF and images after any future corrections to keep the repository consistent.
