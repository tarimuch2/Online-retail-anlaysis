# Online Retail Analysis: Power BI and Excel

Data visualization project completed through the **Tata Consultancy Services Data Visualization Job Simulation on Forage** (Nov 2026). The brief: turn online retail transaction data into insights for a client's CEO and CMO to guide expansion planning.

## Business questions
1. **CEO:** What seasonal trends appear in 2011 monthly revenue, and what do they mean for next year's forecast?
2. **CMO:** Which 10 countries generate the most revenue and units sold (United Kingdom excluded as the established market)?
3. **CMO:** Who are the top 10 customers by revenue?
4. **CEO:** Which regions show the strongest demand for expansion (United Kingdom excluded)?

## Approach
- **Data cleaning (Excel):** Added conditional formulas that flag rows with quantity below 1 (returns) or unit price below $0 (entry errors), then excluded them. Analysis covers 530K clean transactions across 38 countries ($10.7M revenue, Dec 2010 to Dec 2011).
- **Analysis (Excel):** Pivot table and chart of monthly revenue.
- **Visuals (Power BI):** Monthly revenue line chart, top countries, top customers, and a demand map. See `powerbi/online_retail_analysis.pbix`.

## Key findings
| Question | Finding | Business impact |
|---|---|---|
| 1. Seasonality | Revenue held near $685K a month from Jan to Aug, jumped 39% in September, and peaked at $1.51M in November (2.2x the Jan to Aug average). December is incomplete (data ends Dec 9). | The last four months drive the year, so the CEO can plan next year's forecast around a Q4 peak. |
| 2. Top markets | The Netherlands, Ireland, Germany, France and Australia lead outside the UK, together about 70% of non-UK revenue. | Priority markets for expansion spend. |
| 3. Top customers | Top 10 customers account for 14% of revenue; the largest is only 8% above the second. | Low dependence on a few accounts; the CMO gets a clear retention list. |
| 4. Demand map | Sales concentrate in Europe, with little demand in the Americas, Africa and Asia. | Untapped regions to test in an expansion strategy. |

![Monthly revenue](images/q1_monthly_revenue.png)
![Top countries](images/q2_top_countries.png)
![Top customers](images/q3_top_customers.png)
![Country demand](images/q4_country_demand.png)

## Repository contents
- `powerbi/online_retail_analysis.pbix`: Power BI report
- `data/`: summary tables behind each chart (monthly revenue, top countries, top customers)
- `images/`: chart exports

## Tools
Microsoft Excel (conditional formulas, pivot tables, charts), Microsoft Power BI.

## Data
Online Retail dataset provided by the Forage simulation (transactions from a UK-based online retailer, Dec 2010 to Dec 2011). The full raw file is not included here because of its size.
