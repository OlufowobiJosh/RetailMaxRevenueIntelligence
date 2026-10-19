# RetailMax | Insights and Recommendations

## Basis of analysis

These observations come from the four-page saved Power BI report in `reports/RetailMax_PowerBI_Report.pdf`. Values are read from the export rather than recalculated from transaction-level data. Chart rankings describe the visible report context. No calendar year, accounting policy or active filter selection has been established from the export.

## 1. Channel contribution

**Observation:** Online has the largest revenue bar and the largest channel profit bar. Store and Marketplace are smaller and look similar in the displayed comparisons.

**Business implication:** Online is the largest channel in the report, but gross profit alone does not account for fulfilment, marketplace fees, marketing or service costs.

**Recommendation:** Compare channel contribution after these costs. Reconcile completed sales, returns and cancellations before using the figures to allocate marketing spend.

## 2. Product category performance

**Observation:** Home Appliances leads category revenue and has the largest displayed category gross profit bar. Lifestyle follows closely. Electronics and Office Tech generate lower revenue in this view.

**Business implication:** A high revenue category can still have a lower margin or higher operational costs. Revenue rank is only one part of product prioritisation.

**Recommendation:** Compare category-level gross margin, quantities, returns and discount levels. Investigate stock and promotion decisions at product level before changing the category mix.

## 3. Regional performance

**Observation:** West has the highest displayed gross profit, followed by North, South and East on the executive page.

**Business implication:** This identifies where to investigate profit concentration, but the customer page uses labels such as North West and London. The export does not establish whether both charts describe the same geographic dimension.

**Recommendation:** Define the geographic hierarchy, for example store trading region versus customer address region. Compare revenue, margin and customer distribution only after that mapping is clear.

## 4. Monthly revenue profile

**Observation:** February is the lowest point and July is the highest point in the displayed January-to-December revenue profile. The line fluctuates rather than rising consistently.

**Business implication:** This suggests periods worth investigating; it does not establish recurring seasonality. The export does not show whether months combine more than one year.

**Recommendation:** Use a year-month axis, verify the date relationship and compare like-for-like periods before making a seasonal or year-on-year claim.

## 5. Customers and loyalty

**Observation:** Bronze, Silver, Gold and VIP are compared by both revenue and gross profit. Loyalty-member and non-member revenue bars appear similar. The repeat-customer and retention cards display 99.94% and 99.05% respectively.

**Business implication:** Customer counts and loyalty comparisons are useful descriptive views. The very high rates require a definition of qualifying purchases, distinct customers and the observation period before they can support retention decisions.

**Recommendation:** Establish a repeat-purchase rule and a period-based retention cohort. Compare customer value and margin using the same order-status and time filters. Treat loyalty differences as associations unless a suitable evaluation design can support a causal conclusion.

## 6. Discounts and margin

**Observation:** The export displays an average discount of 20.09%, discounted revenue of £110.37 million and discounted profit of £27.18 million. Displayed discounted margin is 24.63%, compared with 24.87% overall, a difference of 0.24 percentage points.

**Business implication:** These values justify investigating pricing and promotion performance. The export does not establish whether "discounted revenue" means net revenue after discount or revenue from discounted transactions only.

**Recommendation:** Define both the discounted and non-discounted populations. Compare like-for-like products, time periods, channels and order statuses. Confirm whether the average discount is an unweighted row average or weighted by quantity or value.

## Proposed next decisions

| Priority | Action | Decision supported |
| --- | --- | --- |
| First | Reconcile revenue, distinct transactions, units and status treatment. | Establish which commercial totals can be relied on. |
| Second | Validate customer measures, blank dimension members and geographic definitions. | Make comparisons consistent across pages. |
| Third | Compare channel and category profitability with relevant costs. | Identify where deeper commercial investigation is most useful. |
| Fourth | Evaluate promotion performance with an appropriate comparison group. | Assess which pricing actions merit testing. |

These are recommendations for further analysis. The report provides no evidence that they were implemented or that any resulting performance improvement was measured.
