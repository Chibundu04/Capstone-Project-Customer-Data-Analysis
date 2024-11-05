## Description
Analysis of customer subscription data to inform business growth strategies.

## Data Collected
- Customer subcription data (33,787 records)
- Variables:
    - Subcription type (Basic, Premium, Standard)
    - Region (North, South, East, West)
    - Revenue
    - Cancellation status (True/False)
 
## Project Objectives
- Identify Key trends in customer subscriptions
- Analyze revenue generation by subscription type
- Determine cancellation rates by region
- Develop recommendations for business growth

## Revenue by subcription type
- Revenue by subscription type
- Cancellation rate  by region
- Top 10 high-value customers

## How to Use the Data  
- Explore data visualization dashboards (Power BI
- Run SQL queries for custom analysis
- Review findings and recommendations report

## Formula Used
- Revenue calculation: SUM(Revenue) by subscription type
- Cancellation rate calculation: COUNT(Canceled) / COUNT(*) * 100 by region

## Tools and Methods Used
- Excel for data cleaning and pivot tables
- SQL for data querying
- Power BI for data visualization

## Power BI Visualizations
# Dashboards
- Subscription Revenue Dashboard
- Cancellation Rate Dashboard
- Top Customers Dashboard

# Reports
- Revenue by Subscription Type Report
- Cancellation Rate by Region Report
- Customer Segmentation Report

## Visualizations
![image](https://github.com/user-attachments/assets/c30b2467-52a4-46d8-8036-f9c0bd1f14c6)

# Revenue by Subscription Type
![image](https://github.com/user-attachments/assets/7ccb3f93-e2c5-48b9-81d8-e3064036308f)

# Cancellation Rate by Region
![image](https://github.com/user-attachments/assets/ffb223e6-dda3-460a-8539-bd8c53524d98)

## Visual Analysis and Inference
![image](https://github.com/user-attachments/assets/a6c7c263-0449-4e6f-9cce-c7ca72d7cb8e)

- Pivot Table 1 - Revenue by Subscription Type
![image](https://github.com/user-attachments/assets/6cf7aef3-3c92-4c35-bce6-f87dc1ec29c8)
 Pivot Table 2 - Cancellation Rate by Region
![image](https://github.com/user-attachments/assets/bf9d9846-1777-450b-8293-7e9587857a42)

## SQL Scripts

# All Customer Data
SQL 
SELECT * FROM [CAPSTONE PROJECT CUSTOMER DATA SET];

## Total Customers By Region
```sql
 SELECT 
    Region, 
    COUNT(CustomerID) AS TotalCustomers 
FROM [CAPSTONE PROJECT CUSTOMER DATA SET]
GROUP BY Region;

---SELECT 
    SubscriptionType,
    SUM(Revenue) AS TotalRevenue
FROM 
    [CAPSTONE PROJECT CUSTOMER DATA SET]
GROUP BY 
    SubscriptionType
ORDER BY 
    TotalRevenue DESC;

-- SELECT 
    Region,
    COUNT(Canceled) AS CancellationCount
FROM 
    [CAPSTONE PROJECT CUSTOMER DATA SET]
WHERE 
    Canceled = 'TRUE'
GROUP BY 
    Region
ORDER BY 
    CancellationCount DESC

# Key Findings
- Basic subscribers generate 2x more revenue than Premium, an increase of 50%
- Average subscription duration is 12 months.
- Cancellation rates are highest among Basic scbcribers (25%).

# Key Takeaways:
- Basic subscribers and East region customers are key revenue drivers
- Cancellation rates vary by region and subscription type
- Customer demographics and industry segmentation can inform targeted marketing.

# Actionable Insights:
- Offer target promotions to Basic subscribers and East region customers
- Develop region-specific retention strategies
- Create indiisty-specific marketing campaigns

# Conclusion
This analysis of customer subscription data provides valuable insights into revenue generation, cancellation rates, and customer segmentation. 

# Repository Maintenance:
This repository will be updated regularly to reflect new data and insights.

