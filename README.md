# Dashboard-Sales-Performance

## Introduction
Retail businesses generate a large amount of customer and transaction data every day, which can be leveraged to support better decision-making. This project aims to analyze overall sales trends, sales and product quantities sold by category, top selling products by sales and quantities, as well as the distribution of sales and product quantities sold across cities. The analysis is performed using SQL in Google BigQuery for data processing and Looker Studio for visualization.


## Tools
- Google BigQuery
- Google Looker Studio
  

## Dataset
|Dataset             |Description                                                              |Column                                                                                                              |
|--------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
|Customers           |Contains information about customer.                                     |CustomerID, FirstName, LastName, CustomerEmail, CustomerPhone, CustomerAddress, CustomerCity, CustomerState, CustomerZip|
|Orders              |Contains information about order transactions.                           |OrderID, Date, CustomerID, ProdNumber, Quantity                                                                     |
|Product Category    |Contains information about product category names.                       |CategoryID, Categoryname, CategoryAbbreviation                                                                      |
|Products            |Contains information about product details                               |ProdNumber, ProdName, Category, Price                                                                               |

##Entity Relationship Diagram

<img width="818" height="682" alt="Entity Relationship Diagram (ERD)" src="https://github.com/user-attachments/assets/cb431c08-c2ba-4aaa-b77e-ff7b946ca6b8" />


## Business Question
- What is the total overall sales generated?
- What is the total sales for each product category?
- What is the total quantity of products sold for each product category?
- How is the distribution of total sales across customer cities?
- What is the total quantity of products sold in each city?
- Which product categories are in the top 5 with the highest sales?
- Which product categories are in the top 5 with the highest quantity sold?


## Process
- Process raw data using SQL in BigQuery to processing data and ensure it is ready for analysis.
- Integrate processed data from Google BigQuery into Google Looker Studio.
- Developing an interactive dashboard to analyze sales performance


## Dashboard Preview

<img width="1198" height="898" alt="image" src="https://github.com/user-attachments/assets/79643c69-e9c0-4a7d-b8fd-139b9a836230" />

Logo Source: Icon made by kmg design from www.flaticon.com


## Insight & Recommendation
- Total sales decreased from 931,204 in 2020 to 841,495 in 2021, representing a decline of 9.63%. Despite the overall annual drop, sales performance in 2021 reached its peak in June, making it the highest-selling month of the year.
- The robot category generated the highest sales at 743.5K despite only 1.1K units sold. Meanwhile, ebooks, training videos, and blueprints recorded higher sales volumes but contributed less than 100 thousand in sales due to their lower price range. This difference in pricing structure and revenue contribution presents an opportunity for the company to implement a bundling strategy by combining high-priced products such as robots or drones with lower priced products like ebooks and training videos.
- Washington recorded the highest sales at 55.381 with a total of 308 products sold. The high demand in this region highlights the importance of optimal stock management to ensure product availability and prevent potential sales loss due to stockouts.
