# Customer Feedback Analysis

Statistical analysis of a customer feedback dataset to test whether issue resolution and feedback length actually relate to customer satisfaction.

## Tools & Techniques
- **Python:** pandas, NumPy, SciPy, statsmodels, Matplotlib, Seaborn
- **Techniques:** data cleaning (missing values, duplicates, outlier checks via boxplots), descriptive statistics, independent-samples t-test, OLS linear regression, group-comparison visualization

## What I Did
1. **Data cleaning:** checked for missing values, duplicates, and data types; used boxplots to confirm no extreme outliers in satisfaction score or feedback length.
2. **Descriptive statistics:** summarized satisfaction score and feedback length overall and by region (mean, median, std).
3. **Hypothesis testing:** ran an independent-samples t-test comparing satisfaction scores between customers whose issues were resolved vs. not resolved.
4. **Regression analysis:** built an OLS model to test whether feedback length predicts satisfaction score.
5. **Visualization:** boxplots comparing satisfaction score and feedback length across issue-resolution groups.

## Key Findings
- **Issue resolution and satisfaction:** the difference in satisfaction scores between the "resolved" and "not resolved" groups was statistically significant (t = -2.066, p = 0.0397). Counter to expectation, customers whose issues were resolved reported slightly *lower* satisfaction than those whose issues weren't — a result worth digging into further (e.g., resolution quality, wait time, or how "resolved" was defined).
- **Feedback length and satisfaction:** feedback length had a very weak, statistically insignificant relationship with satisfaction score (R² = 0.008, p = 0.134) — longer feedback doesn't meaningfully predict satisfaction in this dataset.

## Files
- `customer_feedback_analysis.ipynb` — full analysis notebook
