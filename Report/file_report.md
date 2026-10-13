# Week 1 Project: E-commerce Sales Data Cleaning and Analysis

 1. Project Title and Objective

Project Title: E-commerce Sales Data Cleaning, Analysis, and Visualization

Objective: The objective of this project is to clean an e-commerce sales dataset, calculate important business KPIs, analyze sales trends and customer behavior, and present the results using charts and a dashboard mockup.

 2. Dataset Overview

The dataset contains e-commerce order information, including order date, customer ID, product category, region, quantity, unit price, discount, payment method, delivery days, customer rating, and revenue.

* Rows before cleaning: 5,000
* Rows after cleaning: 4,996
* Columns: 12
* Rows removed: 4

The analysis uses a prepared, messy copy of the dataset. The original dataset was kept unchanged.

 3. Data Cleaning and Preprocessing

The dataset was inspected for missing values, incorrect values, duplicate records, and inconsistent date formats.

The following cleaning steps were performed:

1. Removed 4 rows with missing order dates.
2. Filled missing customer IDs with "Unknown".
3. Filled missing product categories and regions using their most frequent values.
4. Filled missing quantity, unit price, and customer rating using median values.
5. Filled missing payment methods using the most frequent value.
6. Standardized mixed date formats.
7. Replaced zero unit prices with the median unit price.
8. Replaced invalid customer ratings of 0 with the median rating.
9. Checked for invalid quantities, prices, discounts, delivery days, ratings, and revenue.
10. Checked for duplicate rows and repeated order IDs.

After cleaning, the dataset contained 4,996 rows and 12 columns, with no missing cells or duplicate rows.

 4. KPI Summary

The following key performance indicators (KPIs) were calculated from the cleaned dataset.

| KPI                             |       Result |
| ------------------------------- | -----------: |
| Total Revenue                   | 5,107,881.09 |
| Total Orders                    |        4,996 |
| Average Order Value             |     1,022.39 |
| Total Units Sold                |       20,203 |
| Top-Selling Category            |  Electronics |
| Units Sold in Top Category      |        7,112 |
| Top Revenue-Generating Category |  Electronics |
| Revenue from Electronics        | 1,830,224.57 |

The currency unit was not specified in the dataset, so no currency symbol has been added.

 5. Sales Trend Analysis

 Monthly Revenue

Monthly revenue was analyzed to understand how sales changed over time. The highest recorded monthly revenue was 44,728.82 in August 2026.

The dataset contains dates from January 2022 to September 2035. September 2035 is incomplete because the last recorded order date is September 9, 2035, so it should not be directly compared with complete months.


 Category Performance

Electronics generated the highest revenue, followed by Clothing, Home, and Beauty.

| Product Category |      Revenue |
| ---------------- | -----------: |
| Electronics      | 1,830,224.57 |
| Clothing         | 1,531,535.90 |
| Home             |   980,564.48 |
| Beauty           |   765,556.14 |

These results indicate that Electronics was the leading category in both units sold and revenue.

 Regional Performance

| Region |      Revenue |
| ------ | -----------: |
| West   | 1,346,889.82 |
| North  | 1,280,506.19 |
| South  | 1,246,252.68 |
| East   | 1,234,232.40 |

The West region generated the highest revenue, while the East region generated the lowest. The differences between regions were relatively small.

 6. Customer Insights

Customer order frequency was analyzed using customer IDs. Records with an "Unknown" customer ID were excluded from the repeat-customer calculation.

* Known customer IDs: 989
* Repeat customers: 950
* One-time customers: 39
* Repeat-customer rate among known customer IDs: 96.06%

The repeat-customer rate is unusually high and should be interpreted carefully. Further checking is needed to confirm whether the dataset's customer IDs accurately represent individual customers.

The average delivery time was 6.12 days, with a median of 6 days.

 Payment Method Analysis

| Payment Method | Number of Orders |
| -------------- | ---------------: |
| Card           |            2,270 |
| COD            |            1,772 |
| Wallet         |              954 |

Card was the most frequently recorded payment method, followed by COD and Wallet.

 7. Data Visualizations

The following visualizations were created for the project:

1. Monthly Revenue by Category:
 A line chart used to compare monthly revenue trends across categories.
 
![Monthly Revenue by Category](../outputs/Monthly%20Revenue%20by%20Category.png)

2. Revenue by Region: A bar chart used to compare sales performance across regions.
![Revenue by Region](../outputs/Total%20Revenue%20by%20Region.png)

3. Payment Method Distribution: A pie chart showing the distribution of orders by payment method.
![Payment Method Distribution](../outputs/Payment%20Method%20Distribution.png)

4. Dashboard Mockup: A single-page view combining KPI cards and charts for a quick summary of business performance.
![Dashboard Mockup](../outputs/dashboard/dashboard_mockup.png)

The chart images will be included with the project outputs.

 8. Key Findings

1. Total revenue was 5,107,881.09 across 4,996 orders.
2. Electronics was the top category for both units sold and revenue.
3. The West region recorded the highest revenue.
4. Card was the most frequently recorded payment method.
5. The average order value was 1,022.39.
6. The average delivery time was 6.12 days.
7. The calculated repeat-customer rate was 96.06% among known customer IDs, but this needs validation.

 9. Recommendations

1. Review Electronics sales and stock levels because it is the leading category.
2. Investigate the reasons for differences in revenue across regions.
3. Review monthly trends using complete months to identify reliable seasonal patterns.
4. Monitor delivery times and investigate orders with unusually long delivery durations.
5. Validate customer IDs and repeat-customer calculations before using them for business decisions.
6. Keep data-cleaning decisions documented so that the analysis can be reproduced.

 10. Limitations and Assumptions

1. Missing values were filled using mode, median, or "Unknown", depending on the column.
2. Replacing zero prices and invalid ratings with median values may affect the analysis.
3. The dataset does not contain a product name, city, or delivery status column. Therefore, individual top products, city-level analysis, and delivery-status trends could not be calculated.
4. The dataset's currency unit was not specified.
5. The dataset includes an unusually long date range. Dates should be verified before drawing conclusions about seasonality.
6. The repeat-customer rate is based only on known customer IDs and needs validation.
7. This analysis is based on the available dataset and does not establish the causes of observed sales patterns.

 11. Conclusion

This project demonstrated how to clean an e-commerce dataset, calculate business KPIs, examine sales and customer patterns, and create visualizations. Electronics was the leading category by revenue and units sold, and the West region recorded the highest revenue. The results provide a useful overview of the dataset, while the documented limitations highlight areas requiring further validation.
