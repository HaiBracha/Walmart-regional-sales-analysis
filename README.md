Walmart Regional Product Mix and Profitability Analysis
--------------------------------------------------------


## Project Background

Walmart is the largest retailer in the United States, serving a wide variety of customers across thousands of stores. This project analyzes a multi-year, multi-region dataset of 1,500 Walmart stores to answer a critical business question:

How can Walmart optimize its product selection for each region, considering local customer demographics, in order to maximize profits and reduce financial losses caused by product returns?

The analysis is designed to provide actionable, data-driven recommendations for regional managers, product and category teams, and operational leaders at Walmart.


*********************************************************************************************************************************************************************************************************************************************************************************************


## Executive Summary
---------------------


- Total Sales from 2016 to 2025: $20.8 billion across all regions and product categories.

- Total Transactions: 5,408

- Grocery is the leading product category in every region, responsible for 58–64% of sales:

  -  Midwest: 62.08%

  -  Northeast: 58.39%

  -  South: 63.33%

  -  West: 58.08%

- Clothing has the highest return rate (8.4%), with Electronics also elevated (7%).

- Total value lost to returns across all product categories: $751 million.

- Customer Demographics: Most sales come from customers aged 45 to 64 and those with an annual income of $60,000 to $80,000.

- Sales by Gender:

  - Female: $11.0B

  - Male: $9.8B

- Sales by Customer Income Band:

  - $0–20K: $3.06B

  - $20K–40K: $0.84B

  - $40K–60K: $4.21B

  - $60K–80K: $6.91B

  - $80K–100K: $1.65B

  - $100K+: $4.14B

- Profitability is significantly impacted by returns, especially in Clothing and Electronics. Grocery brings in the highest sales with the lowest returns.


*********************************************************************************************************************************************************************************************************************************************************************************************



## Data Overview and Data Model Diagram
----------------------------------------

Data Sources:

This project uses a fictional but realistic dataset representing 1,500 Walmart stores.

The main data tables are:

- Sales – Each row is a sales transaction, linked to product, customer, and store information.
- Products – List of all products, their categories, and units.
- Stores – Each store’s location, assigned region, and city/cost-of-living tier.
- Customers – Each customer’s demographics (age, gender, income, employment status, region).
- Demographics – Detailed demographic information linked to customers and store locations (such as age group, gender, income band, and region).

 <img width="1217" height="360" alt="image" src="https://github.com/user-attachments/assets/3547933c-c53f-4167-b88d-2d00c1574820" />


*********************************************************************************************************************************************************************************************************************************************************************************************



 ## Table Relationships and Keys
 --------------------------------

- Sales → Customers

Key: Customer ID in Sales = CustomerID in Customers

- Sales → Products

Key: Product ID in Sales = ProductID in Products

- Sales → Stores

Key: Store ID in Sales = StoreID in Stores

- Customers → Demographics

Key: City in Customers = City in Demographics

- Demographics → Stores

Key: City in Demographics = City in Stores


*********************************************************************************************************************************************************************************************************************************************************************************************


## Key Insights and Deep Dive
------------------------------

- Sales Performance by Region and Category
   -  Grocery is the largest category across all regions (up to 63% of sales in the South).
   -  Clothing, Electronics, and Beauty have significant but smaller shares, with regional variation.
  <img width="1886" height="967" alt="Screenshot 2025-08-19 210011" src="https://github.com/user-attachments/assets/66896e41-2d10-40cb-939f-bdb4249993fd" />

-------------------------------------------------------------------------------------------------------------------------------------------------------------
- Demographic and Income Trends
   - Customers aged 45–64 and those with annual incomes of $60,000–$80,000 account for the largest share of sales.
   - Female customers slightly outspend males in total sales.
     
   <img width="1919" height="994" alt="Screenshot 2025-08-19 210030" src="https://github.com/user-attachments/assets/0e57dfd8-ba85-4bb9-89a0-b754583836f6" />

--------------------------------------------------------------------------------------------------------------------------------------------------------------
   

- Return Rates and Profitability
   - Clothing has the highest return rate (8.4%), Electronics is next (7%), while Grocery has the lowest (2%).
   - Total value lost to returns across all product categories is 751 million US dollars.

<img width="1916" height="977" alt="Screenshot 2025-08-19 210045" src="https://github.com/user-attachments/assets/3a10366c-c2b3-49e1-974e-b38c25adfb22" />

  ********************************************************************************************************************************************************************************************************************

## Assumptions and Caveats
---------------------------

- This project uses a sample of 1,500 Walmart stores, which represents about 15% of the company’s U.S. locations.

- Store locations, cities, and states are real U.S. places, but the assignment of Walmart stores and some attributes are synthetic for project consistency.

- Customer demographics (age, gender, income, employment status) were generated to reflect real-world distributions but are synthetic.

- Cost-of-living and regional classifications are based on public data but have been adapted for analytical clarity.

- Return rates and return values are calculated directly from product category data in the sales records; there is no separate return transactions table.

- All monetary values are in U.S. dollars and have been rounded for clarity.

  ******************************************************************************************************************************************************************************************************************************************************************************************

## Next Steps and Stakeholder Questions
----------------------------------------

Based on the analysis, the following actions are recommended for key Walmart roles:

- Prioritize Process Improvements in Clothing and Electronics
   - Assigned to: Product Category Managers and Operations Teams
     Clothing and Electronics have the highest return rates and value lost to returns. Category managers and operations should immediately review return policies, product quality, and customer support resources in these categories.

- Review Product Mix by Region
   - Assigned to: Regional Managers and Inventory Planners
     Regional managers should adjust product mix and inventory based on local sales strengths (e.g., focus on Grocery in the South) and reduce high-return categories where they most erode profitability.

- Focus on High-Value Customer Segments
    - Assigned to: Merchandising and Marketing Teams
      Merchandising and marketing should prioritize products, promotions, and in-store experience for customers aged 45–64 and with annual incomes of $60,000–$80,000, who represent the most profitable segments.

- Analyze Underperforming Stores or Regions
    - Assigned to: Regional Managers and Store Performance Analysts
      Identify stores or regions with lower sales and higher returns for targeted review and resource allocation.

******************************************************************************************************************************************************************************************************************************************************************************************

## Potential Follow-Up Questions:
------------------------------

- Are there specific customer groups or regions where returns are unusually high, suggesting the need for targeted interventions by product or customer experience teams?
- Would deeper product-level analysis (such as by brand or price point) help category managers further reduce returns and lost profit?
