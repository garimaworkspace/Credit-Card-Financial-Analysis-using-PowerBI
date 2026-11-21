# Credit Card Financial Analysis

## Project Overview
This project focuses on evaluating credit card client behaviour, transaction patterns, revenue generation, credit utilization and repayment risk to support strategic decisions for a bank's credit card portfolio.

The objective is to analyse customer and card datasets, identify spending and revenue patterns, assess credit risk and churn, and determine which customer segments and card categories offer the strongest value and the highest risk.

Two interactive Power BI dashboards are developed to present key business metrics, supported by a 15-question DAX analysis covering transactions, revenue, risk, retention and customer experience.

## Dashboard Preview

### Credit Card Transaction Report
<img width="6150" height="3525" alt="Transaction Report Dashboard" src="https://github.com/user-attachments/assets/5d1a6255-542f-4c5b-b1b5-e11f0bf0a76f" />

### Credit Card Customer Report
<img width="6150" height="3525" alt="Customer Report Dashboard" src="https://github.com/user-attachments/assets/3754f461-0721-47df-894e-d6b89759a04a" />


## Business Objectives
- Analyse transaction amount, revenue and interest trends across 2023.
- Evaluate credit utilization, delinquency and revolving balances.
- Understand customer behaviour across age, income, education, marital status and state.
- Measure customer acquisition cost and revenue contribution by card category.
- Identify high-risk, high-utilization and churned clients.
- Assess customer satisfaction and the relationship between income, credit limit and loans.

## Dashboard Modules
The project is structured around two dashboards and a DAX analysis:

### 1. Transaction Report
- Revenue, transaction amount, total interest and transaction count
- Quarterly revenue and total transactions
- Revenue by card category (Blue, Silver, Gold, Platinum)
- Revenue by use chip (Swipe, Chip, Online)
- Revenue by expenditure type, education level and customer job
- Card category summary table

### 2. Customer Report
- Revenue, income, total interest and satisfaction score
- Weekly revenue trend
- Revenue by age band, marital status and number of dependents
- Revenue by income group, education and top 5 states
- Gender-wise split across every chart
- Revenue and income by customer job

### 3. DAX Analysis (15 Questions)
- Running total of transactions, 4-week moving average of credit limit, MoM and WoW growth
- Customer acquisition cost ratio and yearly average utilization
- Interest earned versus revolving balance and top 5 clients
- Clients above 80% utilization and customer churn indicator
- Delinquency rate and credit risk score
- Income versus credit limit correlation
- Satisfaction by card category and loan approval versus credit limit
- High-risk client flag

## Dataset Description
The project uses four source files, combined into two model tables:

| Dataset | Description |
|---------|-------------|
| customer.csv | Customer profiles: age, gender, income, education, job, marital status, dependents, loan status and satisfaction score |
| cust_add.csv | Additional customer records appended to the main customer file |
| credit_card.csv | Card details: category, credit limit, transactions, utilization, interest, annual fees, delinquency and weekly date |
| cc_add.csv | Additional card records appended to the main credit card file |

## Dataset Statistics
- 10,293 unique clients after combining the files
- 185 additional records appended from each add-on file
- 4 card categories: Blue, Silver, Gold and Platinum
- Analysis year: 2023 (53 weeks)
- ₹4.55 Cr total transaction amount and ₹5.65 Cr total revenue
- ₹8.90 Cr total credit limit and ₹1.20 Cr revolving balance
- 2 dashboards and 15 DAX analysis questions

## Data Model
- **Customer** and **Credit_Card** tables linked on Client_Num (1:1)
- **Calendar** table built in DAX and linked to Credit_Card by date (1:many)

## Tools & Technologies
- **Power BI Desktop:** Data modelling, interactive dashboards, slicers and visuals
- **DAX:** Calculated columns and measures for time intelligence, ranking, correlation and risk scoring
- **Power Query:** Data cleaning and appending of source files
- **CSV Datasets:** Structured data for customer and credit card analysis

## Key Findings
- Revenue depends heavily on Blue cards (83.5%) and on swipe payments (63.1%).
- Spend is steady but flat, with no consistent growth through 2023.
- Clients aged 40–60 generate about 77% of revenue.
- 49.2% of clients show no spend in the last six months; Platinum has the highest churn (65.7%).
- 6.06% of clients have a delinquent account, similar across all card types.
- 467 clients use more than 80% of their limit, 464 of them on Blue cards.
- Platinum has the lowest satisfaction score (2.72 out of 5).
- Income explains only 1.6% of variation in credit limit (correlation 0.13).

## Expected Business Outcomes
The analysis aims to provide insights into:
- Spending and revenue patterns across customer segments and card categories.
- Credit risk exposure through utilization, delinquency and risk scoring.
- Customer retention challenges and win-back priorities.
- Customer satisfaction gaps across card tiers.
- Credit limit policy and loan-approval decisions.

These insights can support retention campaigns, risk monitoring, limit policy review and customer-experience improvements.

**Project Domain:** Data Analytics | Banking & Credit Cards | Business Intelligence | Financial Analysis
