# Customer Segmentation Analysis for Subscription Service

## Project Overview

This project analyzes customer data from a subscription service to identify customer segments, trends in cancellations and renewals, and patterns in subscription types. The analysis results in a Power BI dashboard that provides actionable insights for stakeholders, enabling data-driven decisions to enhance customer retention and revenue growth.

## Project Goals

1. **Identify Key Customer Segments**: Uncover patterns in subscription types and durations.
2. **Analyze Cancellations and Renewals**: Discover trends and possible drivers behind cancellations and renewals.
3. **Create Interactive Visuals**: Use Power BI to build a dashboard with interactive data filtering for in-depth analysis.

## Tools and Technologies

- **Excel**: Data summarization and pivot table analysis.
- **SQL**: Data extraction and analysis to answer key business questions.
- **Power BI**: Visualization and dashboard creation for stakeholder review.

## Repository Structure

- `data/`: Contains raw data files (e.g., `subscription_data.csv`).
- `excel/`: Excel analysis file (`subscription_analysis.xlsx`) with pivot tables for initial exploration.
- `sql/`: SQL scripts used to extract insights and answer key business questions.
- `power_bi/`: Power BI dashboard file (`subscription_dashboard.pbix`).
- `reports/`: Findings and recommendations generated from the analysis.

---

## Project Instructions

### 1. Excel Analysis

**Objective**: Use pivot tables to identify patterns in subscription types and durations.

#### Steps:
- Calculate the average subscription duration.
- Identify the most popular subscription types.
- Generate additional reports to reveal trends in the dataset.

### 2. SQL Analysis

**Objective**: Extract key insights using SQL queries.

#### Steps:
- **Customer Distribution by Region**: Calculate the total number of customers from each region.
- **Subscription Popularity**: Identify popular subscription types.
- **Customer Cancellations**: Retrieve customers who canceled within six months.
- **Average Subscription Duration**: Calculate the average duration of subscriptions.
- **Long-Term Subscribers**: Find customers with subscriptions longer than 12 months.
- **Revenue Calculation**: Calculate total revenue by subscription type.
- **Regional Cancellations**: Identify the top three regions by cancellation rate.
- **Subscription Status**: Count active and canceled subscriptions.

### 3. Power BI Dashboard

**Objective**: Visualize customer segments, cancellation rates, and subscription trends.

#### Dashboard Visualizations:
- **Subscription Types by Popularity**: Bar chart showing the popularity of subscription types.
- **Cancellations by Region**: Heat map or column chart displaying regional cancellations.
- **Subscription Duration Distribution**: Histogram of average subscription durations.
- **Revenue by Subscription Type**: Pie or donut chart illustrating revenue by subscription type.
- **Active vs. Canceled Subscriptions**: Stacked bar chart comparing active and canceled subscriptions.
- **Top Regions by Cancellations**: Ranking chart of the top three regions with the highest cancellation rates.
- **Interactive Slicers**: Filters for region, subscription type, and status to allow stakeholders to explore the data.

---

## Findings

From the data analysis and dashboard insights:

- **Popular Subscription Types**: Short-term plans are most common, indicating that customers may be hesitant to commit to long-term plans.
- **High Cancellation Rate in Specific Regions**: Certain regions have higher cancellation rates, especially within the first six months.
- **Revenue Distribution**: A few subscription types contribute most to the revenue, suggesting potential for pricing strategy adjustments.
- **Long-Term Subscribers**: A smaller segment maintains subscriptions beyond 12 months, indicating possible brand loyalty within this group.

## Recommendations

Based on the findings, here are targeted recommendations to improve customer retention and revenue:

- **Targeted Retention Efforts**: Implement customer retention strategies in high-cancellation regions, possibly using personalized offers or incentives.
- **Expand Popular Subscription Types**: Introduce variations of popular plans to cater to a wider audience and potentially increase revenue.
- **Loyalty Programs**: Develop programs for customers with subscriptions over 12 months to encourage long-term engagement.
- **Market Analysis for High-Cancellation Segments**: Conduct further analysis to address high cancellation rates and improve customer satisfaction.

---

## Project Deliverables

- **Excel Reports**: Summary reports and pivot tables showing key metrics.
- **SQL Scripts**: Queries to extract and analyze customer data.
- **Power BI Dashboard**: An interactive dashboard with slicers for stakeholder review.

---

