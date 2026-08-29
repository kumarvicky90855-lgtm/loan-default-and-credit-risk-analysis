# Loan Default & Credit Risk Analysis
Loan default and credit risk analysis with an interactive dashboard to identify high-risk borrower segments, key default drivers, and pricing gaps using SQL Server and Excel.
![Dashboard Preview]("Loan_Default_And_Credit_Risk_Analysis_Dashboard_Screenshoot.png") 
## Objective
The objective of this project is to analyze loan default and credit risk data, identify the borrower segments and loan types with the highest default risk, and understand whether interest rate pricing reflects that risk.
## Dataset
Credit Risk Dataset — Kaggle (laotse/credit-risk-dataset), used for risk assessment, data cleaning, analysis, and dashboard development.
The dataset contains 32,574 loan records with information such as loan grade, interest rate, loan intent, home ownership, income, and default status.
## Tools Used
* SQL Server Management Studio (SSMS)
* Microsoft Excel
* Pivot Tables
* Charts
* Excel Dashboard
## Files in this repo
* `01_Loan_Default_&_credit_risk_Analysis_Uncleaned_dataset.csv` — raw loan default and credit risk dataset
* `02_Loan_Default_And_Credit_Risk_Analysis_Dashboard.xlsx` — interactive Excel dashboard
* `03_Loan_Default_and_credit_risk_key_finding_business_analysis.docx` — detailed key findings and business analysis
* `04_Loan_Default_And_Credit_Risk_Analysis_Business_Report.docx` — final project report
* `05_Data_Profiling_and_Transformation_sheet.docx` — data profiling and transformation steps
* `06_Data_Validation_Sheet.docx` — data validation checks
## Methodology
* Reviewed and cleaned the raw loan dataset using SQL Server Management Studio (SSMS).
* Generated a unique loan_id for every record, since the raw dataset had no identifier column.
* Flagged outliers instead of deleting them, and filled missing values using the grade-wise median.
* Built a clean analysis table with derived fields such as Income Band, Age Band, and High-Risk Grade Flag.
* Used Pivot Tables and charts in Excel to summarize the risk data.
* Analyzed default rate by loan grade, home ownership, loan intent, and risk category.
* Developed an interactive Excel dashboard to make the results easier to understand.
## Key Findings
* Grade A loans default only 9.96% of the time, while Grade G loans default 98.44% of the time — almost all of them.
* Renters default 38% of the time, compared to only 9% for people who own their home.
* Debt consolidation loans default the most, at 28.59%, while business loans default the least, at 14.82%.
* Out of 32,574 loans, 7,107 have defaulted — a 22% default rate, much higher than a normal, healthy rate of 3-5%.
* Only 15% of loans are marked high-risk, but these loans have default rates between 59% and 98%.
* Around 31% of all loans are classified as high-risk (10,081 out of 32,574).
* Grade A loans (9.96% default) and Grade G loans (98.44% default) are both charged around the same interest rate, about 11%.
## Recommendations
* We recommend tightening or restricting lending to Grade F and G borrowers, or requiring extra security before approval.
* We suggest giving more weight to home ownership status during loan approval, given the gap between renter and owner default rates.
* We recommend applying extra checks to debt consolidation applications, as these borrowers may already be in financial trouble.
* A review of overall approval criteria is recommended, since a 22% portfolio-wide default rate points to a systemic issue rather than an isolated one.
* We recommend introducing risk-based pricing so that interest rates rise with loan grade and risk category, instead of staying flat across the board.
## Dashboard
The interactive dashboard provides a clear view of:
* Total loans analyzed and total defaulted loans
* Default rate by loan grade
* Default rate by loan intent
* Default rate by home ownership
* Risk category split (low, medium, high)
* Loans by home ownership type
## Conclusion
This project provides a structured view of loan default and credit risk data and helps identify which borrower segments and loan types carry the highest risk. The analysis can support better loan approval decisions, more accurate risk-based pricing, and closer monitoring of high-risk segments.
The dashboard and supporting analysis can be used as a simple decision-support tool for reviewing credit risk information.
