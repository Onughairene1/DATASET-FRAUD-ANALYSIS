# Credit Card Fraud Detection Analysis Report

## Introduction
This report provides an analysis of a credit card transaction dataset, focusing on identifying and understanding patterns in fraudulent transactions. Credit card fraud detection is vital to safeguard financial assets and prevent unauthorized access to user accounts.

## Dataset Overview
The original dataset contains **283,726 records** and **31 columns**, including anonymized credit card transactions. Important features include:

- **Time**: Elapsed seconds since the first recorded transaction.
- **Amount**: The value of the transaction.
- **Class**: Target variable - '0' for Non-Fraud and `1` for Fraud.
- **V1 to V28**: PCA-transformed features (anonymized for confidentiality).

## Data Cleaning and Transformation
The dataset was relatively clean but required some transformation for better visualization and understanding:

- **Removal of Anonymized Features**: Columns `V1` to `V28` were excluded from the analysis as they were encrypted and non-interpretable for direct insights.
- **Class Label Modification**: Values in the `Class` column were changed:
   `0` - **Non-Fraud**
   `1` - **Fraud**  
  This made the overview of transactions easier to grasp.

## Analysis

### Total Transactions vs Fraudulent Transactions

| Metric                      | Value     |
|----------------------------|-----------|
| Non-Fraudulent Transactions | 283,234   |
| Fraudulent Transactions     | 492       |
| **Fraud Rate**              | **0.173%** |

 **Insight**: The fraudulent transactions recorded were significantly fewer compared to the total number of transactions. The fraud cases were spread across the dataset rather than concentrated at particular periods.

### Transaction Amount Observation
- Most fraudulent transactions involved relatively smaller amounts.
- Non-fraudulent transactions varied widely, including many high-value transactions.

## Visualization
- A **bar chart** was used to visually represent the comparison between fraud and non-fraud transactions.
- A **distribution plot** showed that transaction amounts for fraud cases were generally lower.

## Conclusion
The dataset provided minimal insight as the encrypted values in Columns `V1` to `V28` could not be decrypted, thus preventing deeper analysis into factors influencing fraudulent transactions. Consequently, this limited the identification of key fraud patterns. Although the fraudulent transactions were significantly lower in number compared to non-fraudulent ones, they were spread throughout the dataset over time.

