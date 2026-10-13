# Week 1 Project: E-commerce Sales Data Cleaning and Analysis

 Project Overview

This project focuses on cleaning and analyzing an e-commerce sales dataset. The main purpose is to identify data quality issues, calculate key business performance indicators (KPIs), understand sales and customer patterns, and present the findings using charts and a dashboard mockup.

 Objectives

* Clean missing and invalid data.
* Check for duplicate records and inconsistent values.
* Calculate important sales KPIs.
* Analyze sales by product category, month, region, and payment method.
* Explore customer order frequency.
* Create charts and a dashboard mockup.
* Document findings, recommendations, and limitations.

 Dataset Information

The dataset contains 5,000 rows and 12 columns before cleaning. After cleaning, it contains 4,996 rows and 12 columns.

The columns include order ID, order date, customer ID, product category, region, quantity, unit price, discount, payment method, delivery days, customer rating, and revenue.

A prepared, messy copy of the dataset was used for cleaning and analysis. The original dataset was kept unchanged.

 Tools Used

* Python
* Jupyter Notebook in Visual Studio Code
* Pandas for data cleaning and analysis
* Matplotlib for charts
* CSV files for storing raw and cleaned data
* Markdown for project documentation

 Data Cleaning

The cleaning process included:

* Removing rows with missing order dates.
* Filling missing values using suitable methods.
* Standardizing date formats.
* Replacing zero unit prices and invalid customer ratings.
* Checking invalid values, missing cells, and duplicate records.
* Saving the cleaned dataset separately from the raw dataset.

 Key Results

* Total Revenue: 5,107,881.09
* Total Orders: 4,996
* Average Order Value: 1,022.39
* Total Units Sold: 20,203
* Top-Selling Category: Electronics
* Highest-Revenue Region: West
* Average Delivery Time: 6.12 days

The dataset does not specify a currency unit, so no currency symbol is included.

 Visualizations

The project includes:

* Monthly Revenue by Category — line chart
* Revenue by Region — bar chart
* Payment Method Distribution — pie chart
* Dashboard Mockup — a single-page summary of KPIs and charts

The chart images are saved in the `outputs` folder.

 Project Structure

* `Data/raw/` — original and prepared raw datasets
* `Data/cleaned/` — cleaned dataset
* `notebooks/` — Jupyter Notebook containing the analysis
* `outputs/` — charts and KPI summary
* `outputs/dashboard/` — dashboard mockup image
* `Report/` — final project report
* `README.md` — project overview and instructions

 How to Run

1. Open the project folder in Visual Studio Code.
2. Open the notebook inside the `notebooks` folder.
3. Select the project's Python environment or kernel.
4. Install the required Python libraries if they are not already installed.
5. Run the notebook cells in order to reproduce the cleaning, analysis, and visualizations.

 Limitations

* The dataset does not include product names, city, or delivery status.
* The currency unit is not specified.
* The date range and repeat-customer calculations should be checked before making business decisions.
* Results depend on the quality and completeness of the available data.

 Conclusion

This project demonstrates data cleaning, exploratory sales analysis, KPI calculation, and data visualization using Python. The results highlight product category and regional performance while documenting assumptions and limitations for future improvement.
