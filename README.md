# Plato's Pizza Sales Analysis (Interactive Dashboard creation using MS Excel)

## Table of Contents

- [Project Overview](#project-overview)

- [Data Sources](#data-sources)

- [Recommendations](#recommendations)


### Project Overview

This data analysis project aims to provide insights into the sales performance of Plato's Pizza for the year 2015. By analyzing various aspects of the sales data, I seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.


### Data Sources
Sales Data: The primary dataset used for this analysis is the "Pizza Sales.xlsx" file, containing detailed information about each sale made by Plato's Pizza.
Dataset can be found in Kaggle [download](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)

### Tools Used
Excel 
- Data Cleaning
- Data Analysis with the use of Pivot tables.
- Visualization

### Data Cleaning/Preparation
In the initial data preparation phase, I performed the following tasks:

- Created a new sheet to duplicate the original data for the cleaning.
- Inspected the data for any missing values by using the column header row of each columns.
- Data cleaning and formatting by ensuring the data is consisitent and clean with respect to data types, data format and valued used.
- Added new columns to extract the month and days from the Order date to answer some of the questions for the analysis. The Text function was used for this extraction; =TEXT([@[order_date]],"mmmm") and =TEXT([@[order_date]], "dddd").

![Data Model - Pizza Sales - Excel 1_24_2025 6_40_44 PM](https://github.com/user-attachments/assets/0c609f73-16a6-45ef-b878-164ce9bc763d)


- Added a column to group the order time, created a table and used the Vlookup Function thus =VLOOKUP([@[order_time]],$S$6:$U$30,3,1) for the Hourly Bucket column.
  
 ![Data Model - Pizza Sales - Excel 1_24_2025 5_49_06 PM](https://github.com/user-attachments/assets/a1a5f796-9e63-450a-887a-2d1701d34ecb)

- Created a new sheet to use Pivot Tables for the analysis according to the questions asked.

### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:

- What is the overall sales trend?
- Which category of pizza are customers favorite?
- What are the peak sales periods?
- Plato's top selling pizza types?

### Results/Findings
The Insight to this data are as follows;

- Total Revenue: $ 817.8K
- Total Quantity Sold: 49.5K
- Total Orders: 21.35K
- Average Order Value: $ 38.31
- Fridays are the busiest day of the week with a total of 8,106 orders and a revenue generation of $ 136k
- July was the busiest month with a total of 4,301 orders and a revenue generation of $ 72.5K
- Among the categories of pizza, most of Plato Pizza's customers preferred the Classic with 14,888 quantity sold and generating 27% of its revenue for the year.
- 12pm - 1pm tends to be the busiest time of the day for ordering pizza by their customers.
- Plato's Pizza Top 3 Pizza types are;
  
   The Thai Chicken Pizza
  
   The Barbecue Chicken Pizza
  
   The California Chicken Pizza

  
### Recommendations
Based on the analysis, I recommend the following actions:

Invest in marketing and promotions during peak sales seasons to maximize revenue.
Focus on expanding and promoting products in Category A.
Implement a customer segmentation strategy to target high-LTV customers effectively.
Limitations
I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.

References
SQL for Businesses by werty.
Stack Overflow
