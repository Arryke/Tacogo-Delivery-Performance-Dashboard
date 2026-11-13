# TacoGo Delivery Performance Dashboard
## Overview
TacoGo is a growing taco delivery business seeking to better understand its order and delivery performance across cities. In this project, I worked in the role of a Power BI Analyst to develop a dashboard that brings key business performance indicators together and helps the business team explore patterns in orders, taco sales, revenue, tips, and delivery operations over two years. The dashboard brings together key business performance indicators to provide an overview of orders, revenue, tips, restaurant performance, taco preferences, and delivery operations. The project turns sales and operational data into an interactive reporting solution. Through KPI cards, charts, comparative visuals, and filters, the dashboard allows users to explore performance across restaurants, years, taco types, and months. It is intended to support a clearer understanding of business trends and areas that may require further investigation.

## Project Scope
The dashboard focuses on three main areas:

1. Program Overview:
   
This section provides a high-level summary of sales and delivery performance. It includes:
 - Total orders, total revenue, total tips, average delivery duration, and average delivery distance, including the year-on-year performance for each metric
 - Taco type distribution and Top six restaurants by total orders.
 - Total revenue by taco size and total orders by month.

2. Tip and YoY Trends:
   
This section focuses on tip patterns and year-on-year restaurant performance. It includes:
- Monthly tip trends and Restaurant-level year-on-year comparisons for total revenue, total tips, total orders, average delivery duration, and average distance.

3. Revenue and Delivery:
   
This section examines revenue patterns and delivery operations. It includes:
- Top six restaurants by average delivery duration.
- Total orders by taco size and taco type.
- Total revenue by month. 


Interactive slicers allow users to explore the dashboard by restaurant name, year, and taco type.

## Business Objective: 
The primary objective of the project was to develop a Power BI dashboard that provides the business team with an accessible view of TacoGo's order, sales, and delivery performance over the past two years.
Specifically, the project aimed to:
1. Monitor key business indicators, including total orders, total revenue, total tips, average delivery duration, and average delivery distance.
2.	Examine order volumes across months, restaurants, taco types, and taco sizes.
3.	Compare restaurant performance using order, revenue, tip, and delivery indicators.
4.	Identify monthly patterns in revenue and tips.
5.	Highlight restaurants with comparatively higher average delivery durations for further operational review.
6.	Present business performance information through interactive visualizations to support monitoring and informed business discussions.


## Document Purpose: 
This document provides an overview of the TacoGo Delivery Performance Dashboard, including its business context, objectives, scope, data model, visualisations, key findings, and potential applications. It is intended to help readers understand the analysis presented in the Power BI report and the types of business questions that can be explored using its interactive features.

## Use case:
The dashboard is intended to serve as a reference point for the business team when reviewing sales and delivery performance. Potential stakeholders and applications include:
1.	Business owners and management: Monitor overall orders, revenue, tips, and delivery indicators to support performance reviews and business planning.
2.	Restaurant managers: Compare order volumes and year-on-year performance across restaurants, and identify locations that may require further investigation.
3.	Sales and marketing teams: Examine monthly sales patterns and demand across taco types and sizes to inform sales planning and promotional discussions.
4.	Delivery and operations teams: Review average delivery duration and distance, and identify restaurants with comparatively longer delivery times for operational review.
5.	Finance and performance reporting teams: Track revenue and tip trends, compare performance across periods, and prepare business performance summaries.

These are potential stakeholders and use cases inferred from the project brief and dashboard functionality. They should not be interpreted as confirmation that the dashboard has been deployed by or formally adopted within a real organization.

   
## Skills Demonstrated:
●	Data cleaning and preparation

● Data modelling and relationships

●	Performance monitoring

●	Time Intelligence

●	Data visualization and Interactive dashboard design

●	Communication of data-driven insights

## Data Source:
The data source is one original Excel workbook containing three worksheets, comprising the fact table and dimension tables, ready to load into PowerBI.

FactOrders: This contains 12 columns and 1000 rows of delivery and order-level data, including order date and delivery date, price, tips collected, delivery duration and distance, and so on.

DimRestaurant: This contains 3 columns and 500 rows of restaurant details, including the restaurantID, restaurant name, and location.

DimTaco: This contains 3 columns and 10 rows of information on the Taco delivered, including TacoId, Taco size, and Taco type.

[Click here to download the dataset](https://github.com/Rikky101/Tacogo-Delivery-Performance-Dashboard/blob/main/Taco%20Sales%20Data.xlsx)

## Data Modelling and Analysis: 
Two key transformation steps were carried out in Power BI:
1.	Table relationships: Relationships were established between the relevant tables to connect the datasets and support analysis. The dataset is structured around one fact table, FactOrders, and two dimension tables, DimRestaurant and DimTaco. This arrangement separates order-level activity from descriptive restaurant and taco information and provides a structure for analysing orders by restaurant and product attributes. These steps support consistent date filtering and allow visuals to draw on related information across the model.
  
2. Calendar table creation: A dedicated calendar table was created to support date-based analysis and time-related filtering in the dashboard.


## Data Analysis and Visualization:
The dashboard uses KPI cards, donut charts, bar charts, column charts, a line chart, and a year-on-year comparison table to communicate business performance. The report allows users to examine overall performance and then explore restaurant, product, monthly, and delivery patterns in more detail.

1.	Overall business Performance: TacoGo recorded 1,000 orders, generating $6,908.25 in revenue and $1,806.11 in tips across the two years. However, year-on-year analysis showed a significant decline in 2025, with orders down 56.7%, revenue down 56.4%, and tips down 54.4%. Average delivery duration improved slightly by 1.0%, while average delivery distance increased marginally by 0.7%.

2.	Restaurant Performance: Urban Tacos recorded the highest overall order volume (117) and revenue ($794.50), while Grande Tacos generated the highest tips ($205.75). El Taco Loco recorded the lowest orders (85), revenue ($574.00), and tips ($152.50). La Vida Taco had the shortest average delivery duration (47.05 minutes), while The Taco Stand had the longest (53.56 minutes). These differences are descriptive and should be interpreted in the context of factors that may influence delivery time, rather than treated as direct indicators of restaurant efficiency.
Year-on-year comparisons showed declines across all restaurants. The Taco Stand demonstrated the strongest relative performance, with the smallest declines in orders (35.9%), revenue (32.6%), and tips (32.8%). Taco Time Express recorded the largest decline in orders (68.1%), while Taco Fiesta had the largest declines in revenue (70.6%) and tips (70.2%). La Vida Taco also experienced the largest increase in average delivery duration (19.8%), while Taco Time Express recorded the largest increase in average delivery distance (14.0%).

<p align="center">
  <img src="https://github.com/Rikky101/Tacogo-Delivery-Performance-Dashboard/blob/main/Restaurant_Performance.png" alt="">
</p>

3.	Monthly Revenue and Order Pattern: In 2024, March recorded the highest monthly orders (72) and revenue ($502.00), while February recorded the lowest orders (44) and revenue ($310.25). In 2025, January led with 60 orders and $386.25 in revenue, whereas June recorded the lowest performance, with only three orders and $25.75 in revenue. Overall, 2025 experienced a substantial decline in monthly orders and revenue, particularly from June onwards, compared with the corresponding months in 2024.
   
<p align="center">
  <img src="https://github.com/Rikky101/Tacogo-Delivery-Performance-Dashboard/blob/main/Total_Revenue_and_Orders_by_Month.png" alt="">
</p>     
  	
4.	Taco Performance: Chicken Taco was the strongest overall performer, recording 218 orders, $1,553.25 in revenue, and $412.14 in tips. Beef Taco recorded the lowest performance across these indicators, with 182 orders, $1,197.75 in revenue, and $309.83 in tips.
Year-on-year comparisons revealed declines across all taco categories. Beef Taco demonstrated the strongest relative performance in orders and revenue, with declines of 49.6% and 46.0%, respectively, while Veggie Taco recorded the smallest decline in tips (49.0%). Chicken Taco experienced the largest declines in orders (60.3%) and revenue (60.4%), while Pork Taco recorded the largest decline in tips (57.1%). By size, Large tacos generated higher revenue ($3,871.00) than Regular tacos ($3,037.25), despite recording slightly fewer orders.

<p align="center">
  <img src="https://github.com/Rikky101/Tacogo-Delivery-Performance-Dashboard/blob/main/Tacotype_Distribution.png" alt="">
</p>


Dashboard: [Click here to interact with the dashboard](https://app.powerbi.com/links/j0udf050bL) 

## Recommendation:
Based on the findings, the following recommendations are proposed:
1. Investigate the substantial decline in orders, revenue, and tips in 2025, particularly from June onwards, and review sales strategies, customer engagement, and promotional activities to improve business performance.
2. Investigate the factors contributing to weaker performance at Taco Fiesta and Taco Time Express, while examining the practices that may explain The Taco Stand's comparatively smaller year-on-year declines.
3. Review delivery processes at La Vida Taco to address its increase in average delivery duration. Investigate the increase in average delivery distance at Taco Time Express to identify possible operational or routing concerns.
4. Examine the factors associated with stronger sales periods, particularly March 2024 and January 2025, and consider targeted promotional activities during months with historically lower order volumes and revenue.
5. Investigate the decline in Chicken Taco sales, explore opportunities to sustain demand for Beef Taco, and review customer preferences for Large and Regular taco sizes to inform menu planning, pricing, and inventory decisions.
6. Establish regular monitoring of orders, revenue, tips, restaurant performance, and delivery indicators to identify emerging trends and evaluate the effectiveness of business improvement strategies.
   
## Conclusion:
The dashboard successfully provides an overview of TacoGo’s order, delivery, and sales performance across the two years. It highlights trends in order volumes, revenue, and tips; identifies top-performing restaurants and taco categories; and enables comparison of performance across years and locations. The findings reveal a significant decline in business performance in 2025, providing insights into areas that require further investigation and supporting more informed, data-driven business decisions.

Thank You for Reading!

Contact me: balogunaryke@gmail.com 

