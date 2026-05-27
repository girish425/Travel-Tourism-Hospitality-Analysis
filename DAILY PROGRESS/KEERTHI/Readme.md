Project Overview
================
Project: Travel, Tourism & Hospitality – Customer Retention and Dynamic Pricing Analysis
----------------------------------------------------------------------------------------
The Travel, Tourism & Hospitality – Customer Retention and Dynamic Pricing Analysis project focuses on analyzing hotel booking data to improve customer retention, reduce booking cancellations, and optimize hotel pricing strategies. Hotels often face revenue loss due to frequent booking cancellations and improper pricing during different seasons. This project aims to understand customer booking behavior and support hotels in making smarter business decisions using data analysis and machine learning techniques.

Person 2 — Missing Values & Outlier Treatment
=============================================
My responsibility was to clean and preprocess the dataset before it was used for Exploratory Data Analysis (EDA), Machine Learning, and dashboard development. My work mainly focused on handling missing values, removing unnecessary data, identifying outliers, and preparing a high-quality cleaned dataset for the next stages of the project.

Dataset Used
------------
For this task, I worked on the dataset named cleaned_step1.csv. This dataset contained hotel booking details such as customer information, cancellation status, room pricing (ADR), booking dates, country information, and agent details. After completing the cleaning and preprocessing steps, I saved the final cleaned dataset as cleaned_step2.csv, which was later used for EDA and machine learning tasks.

Technologies Used
-----------------
To complete this work, I used Python along with several data analysis libraries. Pandas was used for data manipulation and handling missing values. NumPy supported numerical operations, while Matplotlib and Seaborn were used for data visualization, especially for identifying outliers using boxplots. The entire work was performed in Jupyter Notebook.

Week 1 – Data Cleaning & Preprocessing
======================================
Dataset Loading and Initial Setup
---------------------------------
During the first week of the project, the hotel booking dataset was loaded into Python for preprocessing and cleaning activities. The dataset contained booking details, customer information, hotel pricing data, cancellation records, and market-related attributes. This step established the foundation for all further analysis and machine learning tasks.

Missing Value Analysis
----------------------
A detailed missing value analysis was performed to identify incomplete or null values within the dataset. The analysis revealed missing data in important columns such as company, agent, and country. Identifying these missing values was necessary to ensure accurate preprocessing and reliable analytical outcomes.

Handling Missing Values in Agent Column
---------------------------------------
The agent column contained numerical values with missing entries. These missing values were handled using the median replacement technique. Median was chosen because it provides stable results and is less affected by extreme values or outliers.

Handling Missing Values in Country Column
-----------------------------------------
The country column contained categorical information related to customer locations. Missing values in this column were replaced using the mode value, representing the most frequently occurring country in the dataset. This helped maintain consistency within the categorical data.

ADR Outlier Detection
---------------------
Outlier detection was performed on the ADR (Average Daily Rate) column to identify abnormal pricing values. Visual analysis techniques were used to detect extreme ADR values that significantly differed from the normal hotel pricing range. Detecting outliers was important because abnormal values can negatively impact data analysis and machine learning performance.

ADR Outlier Removal
-------------------
After identifying abnormal ADR values, extreme pricing records were removed from the dataset. This improved data quality, ensured more realistic pricing representation, and enhanced the reliability of future analysis and predictive models.

Dataset Verification and Export
-------------------------------
After completing the cleaning process, the dataset was verified to ensure that missing values and outliers had been properly handled. The cleaned dataset was then exported for further Exploratory Data Analysis, Machine Learning tasks, and dashboard development.

Company Column Removal
----------------------
The company column contained a very high percentage of missing values. Since the majority of records in this column were empty and contributed little analytical value, the column was removed from the dataset. This improved dataset quality and reduced unnecessary complexity.

Week 2 – Pricing (ADR) & Revenue Analysis
=========================================
ADR Distribution Analysis
-------------------------
During the second week, the focus shifted toward Pricing & Revenue Analysis using ADR (Average Daily Rate) data. ADR distribution analysis was performed to understand hotel pricing behavior and revenue trends across customer bookings.
The analysis helped identify common pricing ranges, pricing concentration levels, and variations in room pricing behavior. It also highlighted the presence of premium or luxury customer segments associated with higher ADR values.
Visualizations such as histogram plots and distribution curves were used to study the overall ADR spread and pricing patterns.

ADR vs Cancellation Analysis
----------------------------
An analysis was conducted to study the relationship between ADR values and booking cancellations. The objective was to understand how pricing influences customer retention and cancellation behavior.
This analysis compared ADR values between canceled and non-canceled bookings and examined customer price sensitivity during higher pricing periods. The results indicated that bookings with higher ADR values showed increased cancellation tendencies, suggesting the importance of balanced pricing strategies.
Boxplots and comparative pricing distributions were used to visualize the relationship between pricing and cancellations.


Week-2 
------
Day-1:Initialize pricing and ADR analysis notebook

Day-2:Perform dataset inspection for ADR analysis

Day-3:Add stay duration and guest count features

Day-4:Analyze ADR distribution and pricing trends

Day--5:Compare ADR patterns with booking cancellations
