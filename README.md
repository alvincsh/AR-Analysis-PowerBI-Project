# <ins>Accounts Receivable Analysis (PowerBI Project)</ins>

## Table of Contents
- [Project Download Link](#project-download-link)
- [Project Dashboard Image](#project-dashboard-image)
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning & Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

---
### Project Download Link
- [Click Here to Download](#)
---

### <ins>Project Dashboard Image</ins>



---

### Project Overview

The aim of this project is to analyze the Accounts Receivables of GHI Sdn Bhd to ascertain its current debt collection performance, make recommendations to improve the debt collection, rank customers by debt & overdue category, and identify key measures such as Total Oustanding Balance and Average Overdue Days.

### Data Sources

In this project, 1 CSV file of fictitious data was obtained from ChatGPT:

- accounts_receivable_data_final_adjusted.csv
- [Click Here to Download the CSV file](#)


### Tools

- PowerBI Desktop - Data Cleaning, Exploratory Data Analysis, Dashboard Report Visualization


### Data Cleaning and Preparation

The initial data preparation phase included the following steps:
1. Data Loading and Inspection
   - Includes enabling "Column Quality" and "Column Profile" under the "View" ribbon and "column profiling based on the entire data set"
2. Selecting the appropriate data type for each column
3. Data Cleansing and Formatting


### Exploratory Data Analysis

EDA involved exploring the datasets to answer several key questions, namely:

- What are the total outstanding balance?
- What are the average overdue days?
- Who are the customers with high outstanding balance?
- How much total outstanding balance is in each overdue days category?
- What recommendations can be made to boost debt collection?
- Which overdue days category should be prioritized for debt collection efforts?


### Data Analysis

The changes performed to the specific data in the "Transform Data" view is as follow:
  1. Parsed Date for Payment Date column to ensure that the Date format can be applied to the column without errors.
     (Select *payment date* column, go to *Transform* ribbon, select *Date* and then *parse*)
  2. Filter *Days Past Due* column to remove '0' days to show only data with outstanding debts
  3. Added Conditional Column titled *Overdue Time Brackets* to sort *Days Past Due* data into 4 categories:
     - "0 to 30"
     - "31 to 60"
     - "61 to 90"
     - "91 plus"
  4. Inserted Suffix "days" to the *Overdue Time Brackets* column to make the data more easily understood
  5. Renamed the new column as *Overdue Category*

### Results

The analysis results are as follows:
1. The total outstanding balance was $348,703
2. The average overdue days is 183 days
3. The customers with high outstanding balance from high to low are DEF Solutions, XYZ Ltd, PQR Enterprises, ABC Corp, and LMN Inc.
4. The total outstanding balance is in each overdue days category are $36,384.38 (61 to 90 days) and $312,318.26 (91 plus days).
5. Most of the debts fall under the *91 plus days* category fall all the customers.
6. DEF Solutions is the customer with the highest outstanding debt balance of $85,549.14 with 93.6% falling under the *91 plus days* category.



### Recommendations:

Based on the analysis, the following actions are recommended:
1. GHI SDN BHD should gear up their debt collection efforts with special attention on those invoices within the *91 plus days* category
2. Negotiating for earlier settlement with the debtors can be done
3. Selling the receivables of stubborn debtors to factoring services can be considered.
4. In the future, early settlement discounts can be offered to reduce late settlements.
5. Customers with better credit score should be sought to reduce reliance on the existing customers.


### Limitations
1. The data is a fictitious data created by ChatGPT
2. The data is limited
3. Information about the company and its business is unknown which makes it hard to determine whether the *average overdue days* is due to the industry the company is in
4. All key data should be compared with the *Industry Average* to make a more accurate assessment which cannot be done given the limited data available.
