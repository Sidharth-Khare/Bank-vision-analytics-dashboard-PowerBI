# Bank Vision Analytics Dashboard

A personal Power BI portfolio project exploring loan performance, borrower characteristics, and credit-risk patterns. This is an analytical exercise, not a production lending model or a bank engagement.

## Dashboard preview

![Loan portfolio overview](Images/01-overview.png)

[Loan performance and risk](Images/02-loan-performance-risk.png) · [Customer insights](Images/03-customer-insights.png) · [Recommendations page](Images/04-key-insights-recommendations.png)

## Business questions

- How do loan volumes, amounts, and observed default rates vary by loan grade?
- Which borrower and loan-purpose segments warrant further investigation?
- How can a dashboard make portfolio monitoring easier?

## Available files

| Deliverable | Link |
| --- | --- |
| Power BI report | [Bank Vision dashboard](PowerBI/Bank_Vision_Analytics_Dashboard.pbix) |
| Dataset | [Loan data CSV](Dataset/bank_loan_data.csv) |
| Project report | [Report PDF](Documentation/BankVision_Project_Report%20%281%29.pdf) |
| Dashboard images | [Screenshots](Images) |

## Results shown in the published dashboard

The overview displays **31,677 loans**, a total loan amount of **306,001,450**, and a **21.55% default rate**. These are dashboard snapshot values; they have not been independently reconciled here against the CSV and DAX measures.

The risk table shows grade A at **9.56%** default and grade B at **15.93%**. Grade G shows **98.44%**, but contains only **64 loans**. Comparisons should account for sample size and the dataset's coverage.

## Interpretation and limitations

- The recommendations page's statement that A/B borrowers have 5–12% default is inconsistent with its own grade B table.
- A 15% target and a proposed 35% debt-to-income cap need an explicit rationale before being presented as policy.
- Verify the definition of the income-ratio field before describing it as debt-to-income: loan amount divided by annual income is different from debt repayments divided by income.
- High observed default in a small segment does not, by itself, justify stopping lending to that segment.
- This project does not demonstrate a deployed intervention, reduced defaults, or realized financial savings. Dataset provenance and label definitions should be documented before external decision use.

## Open the project

1. Download the PBIX and CSV files.
2. Open the PBIX in Power BI Desktop.
3. If the data source path is unavailable, point the relevant Power Query source to the downloaded CSV.
4. Refresh and reconcile row counts, label mapping, and KPI calculations before quoting results.
5. Review the screenshot caveats above; the existing report pages still require those corrections.

**Tools:** Power BI, Power Query, DAX.

[Portfolio](https://github.com/Sidharth-Khare/analystsido-holic)
