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
- Added a column to group the order time, created a table and used the Vlookup Function thus =VLOOKUP([@[order_time]],$S$6:$U$30,3,1) 
- 

### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:

What is the overall sales trend?
Which products are top sellers?
What are the peak sales periods?
Data Analysis
Include some interesting code/features worked with

SELECT * FROM table1
WHERE cond = 2;
Results/Findings
The analysis results are summarized as follows:

The company's sales have been steadily increasing over the past year, with a noticeable peak during the holiday season.
Product Category A is the best-performing category in terms of sales and revenue.
Customer segments with high lifetime value (LTV) should be targeted for marketing efforts.

### Recommendations
Based on the analysis, we recommend the following actions:

Invest in marketing and promotions during peak sales seasons to maximize revenue.
Focus on expanding and promoting products in Category A.
Implement a customer segmentation strategy to target high-LTV customers effectively.
Limitations
I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.

References
SQL for Businesses by werty.
Stack Overflow
