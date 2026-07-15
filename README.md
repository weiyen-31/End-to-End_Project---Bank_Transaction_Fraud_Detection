# Banking Transaction & Fraud Analytics Dashboard

An end-to-end Business Intelligence project built with Power BI to analyze banking transactions, customer demographics and fraud patterns.

The project focuses on transforming transaction data into business insights through dimensional modelling, DAX development, and interactive dashboards that support business monitoring and fraud detection.

## About the Project

Financial institutions process millions of transactions across multiple channels every day. Monitoring transaction behaviour, identifying fraud patterns, and understanding customer demographics are essential for improving operational efficiency and reducing financial risk.

In this project, I developed an end-to-end Business Intelligence solution using Power BI to explore transaction performance, fraud trends, and customer behaviour for January 2025. The dashboard enables users to monitor key metrics, investigate suspicious activity, and identify opportunities for improving customer and risk management strategies. Hence, this project combines transaction analytics, fraud analysis, and customer demographics to provide a more complete view of business performance, unlike traditional banking dashboards that focus solely on transaction volume.

## Business Questions

This dashboard was designed to answer questions such as:

1. How many transactions are processed across the bank?
2. What is the average transaction amount and account balance?
3. What percentage of transactions are fraudulent?
4. Which states record the highest fraud transaction amounts?
5. Which merchant categories are most frequently associated with fraud?
6. Are certain age groups more susceptible to fraud?
7. How do transaction patterns vary throughout the month?
8. What are the characteristics of the bank's customer base?

## Dataset

Source: Kaggle Banking Transaction Dataset

Industry: Banking / Financial Services

The dataset contains transactional and customer information, including:

- Customer_ID
- Customer_Name
- Gender
- Age	
- State
- City
- Bank_Branch
- Account_Type
- Transaction_ID
- Transaction_Date
- Transaction_Time
- Transaction_Amount
- Merchant_ID
- Transaction_Type
- Merchant_Category
- Account_Balance
- Transaction_Device
- Transaction_Location
- Device_Type	Is_Fraud
- Transaction_Currency
- Customer_Contact
- Transaction_Description
- Customer_Email

## Project Workflow

<img width="273" height="626" alt="image" src="https://github.com/user-attachments/assets/f2d8e8a9-5fe8-40b9-8edb-865270d9d16b" />


## Data Preparation

The dataset was initially assessed to evaluate its quality and suitability for analysis.

There are no significant issues related to missing values, duplicate records or inconsistent data types were identified after reviewing the dataset. As a result, the dataset was considered analysis-ready and imported directly into Power BI.

Futhermore, the raw transactional table was transformed into a dimensional model using a staging layer to support scalable reporting and improve model performance

The preparation process included:

1. Designing a Star Schema
2. Building dimension and fact tables
3. Establishing table relationships
4. Preparing the model for DAX calculations

Additional transformations performed using Power Query included:

1. Creating a Date dimension
2. Creating a Time dimension
3. Formatting data types
4. Renaming columns
5. Creating age groups
6. Creating transaction time buckets

## Exploratory Data Analysis

Before building the dashboard, exploratory analysis was performed to understand transaction behaviour and identify fraud-related trends.

- Transactions by Week of Month

  <img width="930" height="522" alt="image" src="https://github.com/user-attachments/assets/2be06ad3-5754-4d93-b283-047cb8ec93aa" />

  Revealed transaction patterns throughout January 2025 and identified periods of increased activity.

- Fraud Transactions by Age Group

  <img width="917" height="516" alt="image" src="https://github.com/user-attachments/assets/b64b7a4c-8937-4ae9-b5c6-d5ac1d044c12" />

  Helped identify age groups that may be more frequently associated with fraudulent transactions.

- Customer Distribution by Age Group

  <img width="903" height="521" alt="image" src="https://github.com/user-attachments/assets/37db8cda-dddb-4df2-adab-af1bc085715e" />

  Provided an overview of the bank's customer demographics.

These findings helped shape the dashboard design and determine the most relevant KPIs for business users.

## Data Model

The final Power BI model follows a Star Schema consisting of:

- 1 Fact Table
- 4 Dimension Tables

<img width="632" height="471" alt="image" src="https://github.com/user-attachments/assets/d72b36d1-ddfa-470a-9af7-da6f674a7ef1" />

Relationships:

<img width="798" height="243" alt="image" src="https://github.com/user-attachments/assets/0f660fed-47c5-40f5-80e4-5868ef2fca45" />

# Dashboard

The report consists of three pages.

1️. Transaction Overview

<img width="886" height="498" alt="image" src="https://github.com/user-attachments/assets/4c1207c1-29e1-4009-ae95-3c421b3609da" />

This page presents the overview of transaction performance across the organization to provide stakeholders

Highlights Include:
- Total Transactions
- Total Transaction Amount
- Average Transaction Amount
- Average Account Balance
- Fraud Rate
- Transactions by Week of Month
- Transactions by Age Group
- Top Branches by Transaction Amount
- Transaction Amount by Merchant Category
- Transaction Amount by Transaction Type
  
2️. Fraud Analytics

<img width="886" height="493" alt="image" src="https://github.com/user-attachments/assets/92957149-078e-440b-9c94-421d027f5b76" />

This page designed to tracking fraud activity and identifying high-risk patterns.

Highlights Include:
- Total Fraud Transactions
- Total Fraud Amount
- Fraud Rate
- Fraud Amount Percentage
- Fraud Transactions by State
- Fraud Transactions by Age Group
- Fraud Transactions by Week
- Fraud Transactions by Merchant Category
- Fraud Transactions by Time Bucket

3️. Customer Demographics

<img width="884" height="489" alt="image" src="https://github.com/user-attachments/assets/e3b1a60a-aa45-4b71-afe2-3f68de751b0d" />

The customer demograhics page helps understand customer characteristics and account behaviour.

Highlights Include:
- Total Customers
- Average Account Balance
- Gender Distribution
- Customers by Age Group
- Average Transaction Amount by Age Group
- Account Balance by Age Group
- Customers by Account Type
- Customers by Device Type

## DAX Measures

Some of the key measures created in this project include:

- Total Transactions
- Total Transaction Amount
- Average Transaction Amount
- Average Account Balance
- Fraud Transactions
- Fraud Rate
- Total Fraud Amount
- Customer Count
- Fraud Percentage

These measures support transaction monitoring, fraud detection, and customer analytics.

## Key Insights

1. 200,000 transactions were processed in January 2025.
2. Transaction activity peaked during Weeks 2 and 4.
3. Fraud transactions represented approximately 5% of all transactions.
4. All fraud transactions were concentrated during the early morning period (00:00:00–06:59:59).
5. Customers aged 35–44 were among the most represented in fraud-related transactions.
6. Customer distribution was relatively balanced across most age groups.
7. Average account balances remained consistent across customer segments.
8. Gender distribution was nearly evenly split between male and female customers.

## Recommendations

Based on the analysis, several opportunities were identified:

1. Implement additional fraud monitoring for high-risk merchant categories.
2. Introduce risk scoring models for customers exhibiting unusual transaction behaviour.
3. Monitor transaction activity during peak periods for anomalies.
4. Develop targeted fraud awareness campaigns for identified customer groups.
5. Implement enhanced fraud monitoring and real-time alerts during the early morning period (00:00–06:59) to identify suspicious activities more effectively.
6. Continue tracking customer and transaction trends to support proactive risk management.

## Tools Used
| Tool | Purpose |
|------|---------|
| Power BI | Dashboard Development |
| Power Query | Data Transformation |
| DAX | Business Calculations |
| Star Schema | Data Modeling |
| GitHub | Version Control & Portfolio |

## Skills Demonstrated
- Data Modeling
- Star Schema Design
- Power Query
- DAX
- Power BI
- Dashboard Design
- Fraud Analytics
- Banking Analytics
- Customer Analytics
- Data Visualization
- Business Intelligence
