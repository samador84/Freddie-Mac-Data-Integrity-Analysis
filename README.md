# Freddie-Mac-Data-Integrity-Analysis
## Summary
This project analyzes a 10% stratified sample (377,995 rows, 71 features) of Freddie Mac mortgage loan records to evaluate borrower demographics, regional loan concentration, and financial risk metrics.

## Key Findings & Data Engineering
- **Outlier Anomaly Detection**: Identified systemic skew caused by placeholder value flags (`9999.00` in tract income ratios) and engineered a sanitization routine (`loan_df_clean`) to normalize ratios from an inflated mean of 7.8 down to 1.2.
- **Geographic Risk Distribution**: California accounted for 15.6% of all borrowers in the dataset—more than double Texas (6.4%).
- **Financial Risk Modeling**: Comparing CA vs. TX revealed that while average annual incomes are relatively similar ($143k vs. $137k), average loan note amounts in CA ($404k) are significantly higher than in TX ($264k), reflecting elevated debt exposure in high-cost housing markets.

## Repository Contents
- [`FreddieLoanMortgage_code.ipynb`](./FreddieLoanMortgage_code.ipynb): Full Python source code including data cleaning pipelines, demographic profiling, and data visualizations.
- [`Freddie_Mac_Final_Report.pdf`](./FreddieLoanMortgage_FinalReport.pdf): The complete analytical report documenting findings, methodology, and visualizations.

## Tools Used
- **Languages & Libraries**: Python, Pandas, NumPy, Seaborn, Matplotlib
- **Environment**: Jupyter Notebooks
