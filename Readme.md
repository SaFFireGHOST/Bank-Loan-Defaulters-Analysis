# Bank Loan Defaulter Dataset Analysis

## Overview
This repository contains an in-depth analysis of a bank loan dataset aimed at identifying patterns and trends in loan approvals and defaults. The analysis focuses on key factors influencing loan outcomes such as client type, loan purpose, industry, and more. Data visualizations created using Tableau are used to present these insights effectively.

## Dataset
The dataset used for this analysis contains several columns, but the final analysis focuses on 20 key columns. Some of the most important include:

- **Name Contract Type**: Type of loan contract (e.g., Cash loans, Revolving loans).
- **Name Client Type**: Type of client (e.g., New or Repeated customer).
- **Name Contract Status**: Loan status (e.g., Accepted, Rejected).
- **Amt Credit**: Credit amount requested.
- **Loan Amount**: Amount of loan requested by the applicant.
- **Occupation Type**: Client's occupation type.
- **Collateral**: Categorizes collateral into ranges (e.g., 0-500K, 500K-1M).

## Preprocessing
Before conducting the analysis, the dataset was preprocessed to ensure data integrity and accuracy. Columns containing more than 40% null values were removed, and missing data in critical fields were handled using various imputation techniques.

### Key Preprocessing Steps:
1. **Null Value Thresholding**: Columns with more than 40% missing values were dropped.
2. **Handling Missing Data**: Specific strategies were employed to manage missing data in essential fields.

For more details, refer to the [`pre_processing.ipynb`](./pre_processing.ipynb) notebook.

## Calculated Fields
To enhance the depth of the analysis, we introduced the following calculated fields:
- **Approval Percentage**: Proportion of loan applications that were approved.
- **Default Percentage**: Proportion of loans that defaulted.
- **Loan Amount Percentage**: Proportion of the total loan amount that was approved.
- **Age**: Categorized age ranges (e.g., Under 20, 20-25, etc.).

## Tasks
The project was divided into three key tasks to focus on different aspects of the loan dataset:

1. **Factors Affecting Default Rates** (T1)
2. **Factors Affecting Approval Rates** (T2)
3. **Comparing Trends Between Approval and Default Rates** (T3)

### Task 1: Factors Affecting Default Rates
This task analyzes how factors such as gender, education, loan type, income, and occupation influence default rates. Key findings include:
- **Gender**: Males have a higher default rate (10.1%) compared to females (7%).
- **Education**: Applicants with lower secondary education have higher default rates.
- **Occupation and Collateral**: Both factors play a significant role in the likelihood of default.

### Task 2: Factors Affecting Approval Rates
This analysis focuses on loan approval rates and how factors like loan type, product type, and seller industry influence approvals. Key insights include:
- **POS Loans**: Highest approval rate (90%).
- **Client Type**: X-sell loans are approved at a higher rate (74.22%) than walk-in loans (48.36%).
- **Industry**: Jewelry and auto technology sectors show high approval rates but are associated with higher default risks.

### Task 3: Comparing Trends Between Approval and Default Rates
This task compares approval and default rates across various categories:
- **Client Type**: New clients tend to have higher approval rates but also higher default risks.
- **Seller Industry**: The jewelry industry exhibits both high approval and high default rates.
- **Loan Purpose**: Loans for urgent needs like car repairs have higher default rates.

## Contributions
- **Koushik Mupparapu**: Preprocessed the dataset, analyzed factors influencing loan default rates (T1), and documented the findings.
- **Ananthula Harshith Reddy**: Focused on loan approval rate analysis (T2), created visualizations, and contributed to documentation.
- **Anirudh Pathaneni**: Analyzed client types, seller industries, and trends between approval and default rates (T3), and contributed visualizations.

## Visualizations
Tableau was used to generate various visualizations, including:
- **Bar Charts**: To compare loan default and approval rates across categories like gender, education, and loan type.
- **Tree Maps**: To show multivariate data such as default rates based on gender, loan type, and education.
- **Highlight Tables**: To quickly identify high-risk categories for loan defaults.

## References
- Dataset: [Kaggle Loan Data](https://www.kaggle.com/datasets/amity024/data-sources)
