## Overview
This document outlines the analysis of a telecommunications company dataset, focusing on customer churn and Customer Lifetime Value (CLV) based on various factors.

## Data Preparation
- The dataset was loaded and initial preprocessing was conducted.
- Irrelevant columns (e.g., 'ID') were dropped.
- Data was encoded using one-hot encoding for categorical variables.

## Survival Analysis
- We performed survival analysis using Weibull, Lognormal, Exponential, and LogLogistic Fitters.
- Akaike Information Criterion (AIC) and Bayesian Information Criterion (BIC) were computed for each model to determine the best fit.
- The Lognormal Fitter was selected based on AIC and BIC.

## Customer Lifetime Value (CLV) Calculation
- CLV was calculated using the Lognormal Fitter.
- A monthly margin of 1000 and a discount rate of 20% were applied.
- The dataset was limited to relevant columns for the CLV analysis.

## Insights from Analysis
1. **Marital Status Impact on CLV**:
   - Married customers tend to have a higher CLV compared to unmarried customers, indicating lower churn risk.
   - Different peaks in the distribution for married and unmarried customers were observed.

2. **Gender-Based Analysis**:
   - Gender showed a less significant impact on CLV.
   - A clearer peak was observed for female customers.

3. **Influence of Education Level**:
   - Varying CLV distributions were noticed across different education levels.
   - Higher CLVs were seen in customers with less education.

4. **Customer Category Correlation**:
   - CLV distribution varied significantly across different customer categories.
   - The 'Plus service' category exhibited the highest CLV.

5. **Internet Service Impact**:
   - Customers without internet service tended to have higher CLV.

## Conclusion
This analysis provides valuable insights into factors affecting customer churn and CLV in a telecommunication company setting. It highlights the importance of considering customer demographics, service types, and additional features like internet service in predicting customer behavior and value.
