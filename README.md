# Customer Subscription Service

## Project Overview

This project analyzes customer data from a subscription service to identify segments, trends in cancellations and renewals, and patterns in subscription types. The analysis results in a Power BI dashboard that provides actionable insights for stakeholders, enabling data-driven decisions to enhance customer retention and revenue growth.

## Project Goals

1. **Identify Key Customer Segments**: Uncover patterns in subscription types and durations.
2. **Analyze Cancellations and Renewals**: Discover trends and possible drivers behind cancellations and renewals.
3. **Create Interactive Visuals**: Use Power BI to build a dashboard.

## Tools and Technologies

- **Excel**: Data summarization and pivot table analysis.

  [Download here](https://microsoft-excel-2016.en.download.it/#google_vignette)

- **SQL**: Data extraction and analysis to answer key business questions.

  [Download here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

- **Power BI**: Visualization and dashboard creation.

  [Download here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)

## Data Source

The data for this project includes customer records from a subscription service database. Each record contains details on subscription type, duration, customer region, start and end dates, cancellation status, and revenue information.

> **Note**: The dataset used in this project is either synthetic or anonymized for privacy. If real data were to be used, privacy considerations such as data masking and anonymization would apply to protect sensitive information.

[The Customer Data](https://github.com/A-Odunayo/Analysis-for-Subscription-Service/blob/main/Customer%20Subscription%20Data.csv)

## Exploratory Data Analysis (EDA)

The EDA was conducted to understand the distribution and relationships within the data before performing detailed analysis. Key steps included:

- **Data Cleaning**: Checked and removal of duplicates and blank spaces.
- **Descriptive Statistics**: Generated summary statistics for subscription durations, cancellations, and revenue distribution.

## Analysis

The main analysis is organized into Excel, SQL, and Power BI tasks to achieve each project goal. Here’s a breakdown:

### 1. Excel Analysis

This [**Pivot tables**](https://github.com/A-Odunayo/Analysis-for-Subscription-Service/blob/main/Pivot%20table.PNG) shows patterns in subscription types.

### 2. SQL Analysis

Some queries were used to extract key insights, see below:

- **Total number of customers from each region**
  ```SQL
  Select Region,Count(CustomerID) As Total_Customers From [dbo].[Customer Data]
  Group by Region
  Order by Total_Customers Desc

- **Popular subscription types**
  ```SQL
  Select Top 1 subscriptionType, Count(CustomerID) As Total_Subscriptions From [dbo].[Customer Data]
  Group by SubscriptionType
  Order by Total_Subscriptions Desc

- **Average duration of subscriptions**
  ```SQL
  Select Avg(Datediff(Month, Subscriptionstart, Subscriptionend)) As Average_Duration
  From [dbo].[Customer Data]
  Where cancellation_status = 'Active'
  
- **Total revenue by subscription type**
  ```SQL
  Select Subscriptiontype, Sum(Revenue) As Total_Revenue From [dbo].[Customer Data]
  Group by SubscriptionType
  Order by Total_revenue DESC;

### 3. Power BI Dashboard

This [**Visualization**](https://github.com/A-Odunayo/Analysis-for-Subscription-Service/blob/main/Visualization%20(Overview).PNG) shows interractive analysis in Power BI Dasshboard, as i used **Bar Chart, Pie Chart, Card, Gauge, Slicer, Column Chart** and **Tables**, to show some metrics as stated below.

- **Subscription Types by Popularity**
- **Cancellations by Region**
- **Subscription Duration Distribution**
- **Revenue by Subscription Type**
- **Active vs. Canceled Subscriptions**
- **Top Regions by Cancellations**

## Findings

From the data analysis and dashboard insights:

- **Cancellation Rate** is higher in the North, South and West.
- **Basic Subscription Types** contribute over 50% of the revenue.
- Certain regions show strong preferences for specific subscription plans

- ## Recommendations

Based on the findings, here are targeted recommendations to improve customer retention and revenue:

- **Targeted Retention Efforts**: Implement customer retention strategies in high-cancellation regions, possibly using personalized offers or incentives.
- **Expand Popular Subscription Types**: Introduce variations of popular plans to cater to a wider audience and potentially increase revenue.
- **Loyalty Programs**: Develop programs for customers with subscriptions over 12 months to encourage long-term engagement.
- **Market Analysis for High-Cancellation Segments**: Conduct further analysis to address high cancellation rates and improve customer satisfaction.

---

🙂

---


