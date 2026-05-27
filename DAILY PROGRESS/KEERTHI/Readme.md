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

Company Column Removal
----------------------
The company column contained a very high percentage of missing values. Since the majority of records in this column were empty and contributed little analytical value, the column was removed from the dataset. This improved dataset quality and reduced unnecessary complexity.

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

Weeky Progress of Person-2
===========================
Week-1
-------
Day-1: Initialized project structure and added hotel booking dataset

Day-2:Loaded cleaned_step1 dataset using pandas

Day-3:Performed missing value analysis on booking dataset

Day-4:Dropped company column due to excessive missing values

Day-5:Handled missing values in agent and country columns

Day-6:Performed ADR outlier detection and removed extreme values

Day-7:Verified cleaned dataset and exported cleaned_step2.csv

Completed week 1 data cleaning and preprocessing tasks

WEEK 2 – Exploratory Data Analysis (EDA) & Statistical Insights
===============================================================

Main Tasks Included:
-------------------
* ADR (Average Daily Rate) Analysis
* Pricing trends
* Revenue behavior
* Price elasticity insights
* Market segment pricing comparison

Week-2 
------
Day-1:Initialize pricing and ADR analysis notebook

Day-2:Perform dataset inspection for ADR analysis

Day-3:Add stay duration and guest count features

Day-4:Analyze ADR distribution and pricing trends

Day--5:Compare ADR patterns with booking cancellations
