# Textile Business Insights & Commission Analysis

A project based on my freelance work as a Data Engineer at Softwood Textile Company, which integrates data cleaning, business analysis, dashboards, and exploratory machine learning to gain insights into textile contracts and commission-based revenue.

## Problem

The contract data contained duplicate records, negative quantities and commission values, suspicious exchange rates, and inconsistent numeric formats. These issues needed to be addressed before comparing business partners or estimating commissions.

The analysis focused on three questions:

- Which suppliers and customers contributed the most commission?
- What did contract volumes, payment terms, and commission patterns reveal?
- Could the historical records support commission prediction?

## Approach

- Cleaned the data by renaming unclear columns, removing redundant fields and duplicate rows, and filtering invalid values. The cleaned dataset contained **4,614 records and 24 columns**.
- Built interactive dashboards to compare suppliers, customers, product styles, payment terms, and commission patterns.
- Created date-based features and compared Linear Regression, Random Forest, Gradient Boosting, and Support Vector Regression for commission prediction.

## Key Findings

- The cleaned records covered **104 suppliers and 78 customers**, with approximately **$7.91 million in recorded commissions**. This represents the historical business activity analysed.
- **Samad Rubber** contributed the highest total supplier commission, while **Takko** contributed the highest total customer commission.
- **Tiffosi** had the most contract records, showing that the customer with the highest order count differed from the highest commission contributor.
- Average payment terms were **64.9 days**, providing a baseline for reviewing payment processes and cash-flow planning.

## Proposed Solution & Business Value

The analysis recommends strengthening key partner relationships, expanding the customer base to reduce dependency, improving payment processes, and monitoring currency exposure. It also suggests targeting customers with profiles similar to those of existing, high-performing partners.

The project delivered clean data, dashboards, and recommendations to support partner prioritization, commission reporting, and customer expansion planning. Revenue growth, cost savings, and broader market benefits were not quantified in the scope of the work performed.

## Commission Prediction

Gradient boosting achieved the highest reported test **R² of 0.9865**. A caveat remains: inputs derived from commissions risk inflating predictive performance, and subsequent scenario tests employ inconsistent scales. Further validation is required before the model is used for new deals.

**Tools:** Python, pandas, NumPy, Plotly, Matplotlib, Seaborn, and scikit-learn.

**Data privacy:** The original and cleaned datasets are excluded for confidentiality. The notebooks document the workflow and saved results; rerunning them requires access to the private data.
