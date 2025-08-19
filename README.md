Walmart Regional Product Mix and Profitability Analysis
--------------------------------------------------------


** Project Background

Walmart is the largest retailer in the United States, serving a wide variety of customers across thousands of stores. This project analyzes a multi-year, multi-region dataset of 1,500 Walmart stores to answer a critical business question:

How can Walmart optimize its product selection for each region, considering local customer demographics, in order to maximize profits and reduce financial losses caused by product returns?

The analysis is designed to provide actionable, data-driven recommendations for regional managers, product and category teams, and operational leaders at Walmart.


*********************************************************************************************************************************************************************************************************************************************************************************************


** Executive Summary
---------------------

- Total Sales from 2016 to 2025: 21 billion US dollars across all regions and product categories.

- Grocery is the leading product category in every region, responsible for 58–65% of sales.

- Clothing has the highest return rate (8.4%), with Electronics also elevated (7%).

- Total value lost to returns across all product categories: 751 million US dollars.

- Customer Demographics: Most sales come from customers aged 45 to 64 and those with an annual income of $60,000 to $80,000.

- Profitability is significantly impacted by returns, especially in Clothing and Electronics. Grocery brings in the highest sales with the lowest returns.


*********************************************************************************************************************************************************************************************************************************************************************************************



** Data Overview and Data Model Diagram
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



 ** Table Relationships and Keys
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


** Key Insights and Deep Dive
------------------------------

- Sales Performance by Region and Category
   -  Grocery is the largest category across all regions (up to 65% of sales in the Northeast).
   -  Clothing, Electronics, and Beauty have significant but smaller shares, with regional variation.
   <img width="1464" height="522" alt="Screenshot 2025-08-19 124324" src="https://github.com/user-attachments/assets/b820e290-33f2-4823-bcd7-c604096517f8" />

- Demographic and Income Trends
   - Customers aged 45–64 and those with annual incomes of $60,000–$80,000 account for the largest share of sales.
   - Female customers slightly outspend males in total sales.
     
   <img width="381" height="672" alt="Screenshot 2025-08-19 115730" src="https://github.com/user-attachments/assets/ef7d794f-1571-4b92-921b-9c3cbc50a3c9" />
   <img width="769" height="251" alt="Screenshot 2025-08-19 115813" src="https://github.com/user-attachments/assets/9e8a4e4a-a1b9-47ff-a7e1-f727c7bd3c04" />

- Return Rates and Profitability
   - Clothing has the highest return rate (8.4%), Electronics is next (7%), while Grocery has the lowest (2%).
   - Total value lost to returns across all product categories is 751 million US dollars.
     
  <img width="1384" height="458" alt="Screenshot 2025-08-19 124843" src="https://github.com/user-attachments/assets/618aa285-7178-4a23-974b-929223c4f102" />
  <img width="1441" height="432" alt="Screenshot 2025-08-19 124857" src="https://github.com/user-attachments/assets/cda52bd3-3bfd-44af-ac5e-2af6dcb02e7a" />

