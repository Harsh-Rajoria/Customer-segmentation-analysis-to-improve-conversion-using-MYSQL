# Customer-segmentation-analysis-to-improve-conversion-using-MYSQL
### Customer Segmentation and Product Recommendation Analysis Report

#### 1. Data Loading and Initial Inspection
- **TRANSACTION_LINE Table:**
  - Contains transaction data including fields like CUSTOMER_ID, ACCOUNT_CATEGORY, FICO_SCORE, ACCOUNT_BALANCE, TENURE_MONTHS, etc.

- **USER_DATA Table:**
  - Contains user-specific data.

#### 2. Data Cleaning and Exploratory Data Analysis (EDA)
- **Summary of Active vs Closed Accounts:**
  - Counts the number of active and closed accounts.
  - Results: 
    - Active accounts: X
    - Closed accounts: Y

- **Breakdown of Account Types and Balances:**
  - Summarizes total balances across different account categories.
  - Results: 
    - Account Type A: Total Balance X
    - Account Type B: Total Balance Y

- **Loan Amounts vs. Account Balances:**
  - Compares sanctioned loan amounts with current account balances.
  - Insights:
    - Sanctioned Amount X, Account Balance Y
    - Patterns or anomalies observed in balances relative to sanctioned amounts.

- **Closure Percentages for Different Loan Types by Ownership Type:**
  - Calculates closure rates for various loan types and ownership types.
  - Results:
    - Loan Type A, Ownership Type X: Z% closure rate
    - Loan Type B, Ownership Type Y: W% closure rate

#### 3. Customer Segmentation
- **FICO Score Segmentation:**
  - Segments customers based on FICO scores and calculates the percentage of customers in each segment.
  - Segments:
    - Very Poor (300-549): X% of customers
    - Poor (550-649): Y% of customers
    - Fair (650-749): Z% of customers
    - Good (750-849): W% of customers
    - Excellent (850-949): V% of customers

- **Product Usage Segmentation:**
  - Categorizes customers by the types of accounts they hold (e.g., Auto Loans, Credit Cards, etc.).
  - Segments:
    - Auto Loan Only: X% of customers
    - Consumer Loan Only: Y% of customers
    - Combinations: Various percentages based on combinations of account types

- **Account Activity Segmentation:**
  - Segments customers by the status of their accounts (active vs. closed).
  - Segments:
    - Fully Active: X% of customers
    - Mostly Active: Y% of customers
    - Balanced: Z% of customers
    - Mostly Inactive: W% of customers
    - Fully Inactive: V% of customers

#### 4. Cohort Analysis for Customer Retention
- **Cohort Creation:**
  - Categorizes customers into cohorts based on their account opening dates and analyzes how these cohorts have behaved over time.
  - Insights:
    - Cohort Month X: Y% retention rate after 12 months
    - Patterns in retention rates across different cohorts and account categories.

#### 5. Common Account Combinations and Product Recommendations
- **Common Account Combinations:**
  - Identifies common combinations of account types held by customers.
  - Most common combinations:
    - Combination A: X customers
    - Combination B: Y customers

- **Predicting Likely Next Products:**
  - Based on product holding patterns and customer behavior within cohorts.
  - Recommendations:
    - High FICO score customers without a credit card: Recommend Credit Card
    - High balance customers without an investment account: Recommend Investment Account
    - Long-term customers without a loan product: Recommend Loan Product
  - Prioritized high-value customers based on total balance and FICO score.
