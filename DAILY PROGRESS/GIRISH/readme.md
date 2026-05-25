# Progress Report – Person 1  
## Data Acquisition, Initial Cleaning & Exploratory Data Analysis (EDA)

---

# Overview
This report summarizes the contributions completed by **Person 1** during **Week 1** and **Week 2** of the project.  
The primary focus of these tasks was on:

- Setting up the project environment
- Organizing the repository structure
- Loading and understanding the dataset
- Performing data cleaning operations
- Conducting Exploratory Data Analysis (EDA)
- Creating meaningful visualizations
- Identifying important business insights from the dataset

  The work completed during these weeks established a strong foundation for further analysis, dashboard development, and predictive modeling.

---

# Week 1 Tasks Completed

## 1. Repository & Project Setup

The initial phase of the project involved creating and organizing the development environment to ensure smooth collaboration and efficient workflow management.

### Tasks Performed
- Created a GitHub repository for project version control
- Initialized the repository with necessary project files
- Organized the folder structure for better maintainability
- Created separate folders for:
  - Raw datasets
  - Cleaned datasets
  - Jupyter notebooks
  - Reports
  - Visualizations
- Uploaded the dataset into the `raw_data` folder
- Configured the Jupyter Notebook environment for data analysis
- Installed and verified required Python libraries and dependencies
- Prepared the environment for collaborative team development

  ### Outcome
A well-structured and organized project environment was successfully established, enabling efficient project execution and team collaboration.

---

## 2. Dataset Loading & Initial Inspection

The dataset was imported and carefully examined to understand its structure, quality, and available features before performing any transformations.

### Tasks Performed
- Imported the dataset using the Pandas library
- Loaded the dataset into a Jupyter Notebook for analysis
- Performed initial inspection using:
  - `.head()`
  - `.info()`
  - `.describe()`
  - `.shape()`
- Checked:
  - Total number of rows and columns
  - Column names and feature descriptions
  - Data types of all variables
  - Missing values
  - Unique values in categorical columns
- Identified numerical and categorical features separately
- Verified overall dataset consistency and readability

### Outcome
Successfully understood the structure and characteristics of the dataset, which helped in planning the data cleaning and analysis process.

---

## 3. Data Cleaning

Data cleaning was performed to improve dataset quality and ensure accurate analysis results.

### Tasks Performed
- Identified duplicate records in the dataset
- Removed duplicate rows to prevent biased analysis
- Verified dataset integrity after cleaning
- Checked for inconsistencies in column values
- Handled formatting issues and ensured data consistency
- Validated cleaned dataset dimensions
- Ensured the dataset was ready for Exploratory Data Analysis (EDA)

### Outcome
The dataset was successfully cleaned and prepared for further statistical analysis and visualization.

---

# Week 2 Tasks Completed

## 1. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to discover patterns, trends, and relationships within the dataset.

### Tasks Performed

### Univariate Analysis
Performed detailed analysis on individual variables to understand:
- Distribution of bookings
- Frequency of customer types
- Cancellation counts
- Seasonal trends
- Booking lead time distributions

### Booking Trend Analysis
- Explored booking trends across different months and seasons
- Identified peak booking periods
- Analyzed customer reservation behavior over time

### Cancellation Analysis
- Examined cancellation frequencies and patterns
- Identified factors contributing to booking cancellations
- Compared canceled and non-canceled bookings

### Lead Time Analysis
- Studied the relationship between lead time and cancellations
- Analyzed customer booking behavior based on reservation timing
- Observed how advance bookings impacted cancellation probability

### Customer Behavior Analysis
- Investigated customer stay preferences
- Analyzed repeat customer behavior
- Studied booking channel distributions and customer segments

### Outcome
EDA helped uncover meaningful insights, hidden patterns, and important variables influencing hotel booking behavior and cancellations.

---

# 2. Data Visualization

Several visualizations were created to better understand the dataset and present insights effectively.

## Visualization Tools Used
- Matplotlib
- Seaborn

---

## Visualizations Created

### Histograms
Histograms were used to:
- Understand the distribution and shape of numerical data
- Identify skewness in variables
- Detect potential outliers
- Analyze frequency distribution patterns

### Countplots
Countplots were created to:
- Compare categorical variable frequencies
- Analyze customer categories
- Observe booking distributions
- Visualize cancellation counts

### Boxplots
Boxplots were used to:
- Identify outliers
- Compare data spread
- Analyze distribution variations
- Understand booking behavior differences

### Correlation Heatmaps
Correlation heatmaps helped:
- Identify relationships between numerical variables
- Detect highly correlated features
- Understand dependencies among variables
- Support future predictive modeling tasks

### Outcome
The visualizations provided clear and meaningful insights into customer behavior, booking trends, and cancellation patterns.

---

# Statistical Observations & Insights

Several important observations were identified during the analysis process.

## Key Findings

### Booking Cancellations
- Certain variables showed strong influence on booking cancellations
- Higher lead times were associated with increased cancellation probability
- Some customer segments displayed higher cancellation rates

### Seasonal Trends
- Peak booking activity was observed during specific months
- Seasonal demand fluctuations significantly impacted reservations

### Customer Booking Behavior
- Advance booking behavior varied among customers
- Repeat customers showed different booking patterns compared to new customers
- Stay duration and reservation timing influenced booking outcomes

### Data Relationships
- Correlation analysis revealed important feature relationships
- Some numerical variables showed moderate to strong correlations

### Overall Insight
The analysis successfully highlighted critical business trends and customer behavior patterns that can support future dashboard development and predictive analytics.

---

# Technologies Used

The following technologies and tools were utilized throughout the project:

-Python

-Pandas

-NumPy

-Matplotlib

-Seaborn

-Jupyter Notebook

-GitHub

---

# Conclusion

During Week 1 and Week 2, significant progress was made in establishing the project environment, cleaning the dataset, and performing exploratory analysis.

The completed tasks provided:
- A clean and structured dataset
- Strong understanding of booking behavior
- Valuable insights into cancellation patterns
- Effective visual representation of trends and relationships
