# Week 2 – Day-to-Day Progress Report

## Exploratory Data Analysis (EDA) on Hotel Booking Dataset

---

# Day 1 – Understanding the Dataset & Initial Exploration

### Work Done

The first day focused on understanding the structure of the dataset and preparing it for analysis. The dataset was loaded and inspected to identify the number of rows, columns, data types, and missing values.

Basic statistical summaries were generated to understand numerical features such as ADR, lead time, and booking counts.

### Key Activities

* Loaded the cleaned dataset
* Checked dataset shape and column information
* Analyzed missing values
* Generated descriptive statistics
* Identified important columns for EDA

### Code

```python
import pandas as pd

# Load dataset
df = pd.read_csv("hotel_bookings_cleaned.csv")

# Display dataset information
print(df.info())

# Check missing values
print(df.isnull().sum())

# Statistical summary
print(df.describe())
```

---

# Day 2 – Monthly Booking Trend Analysis

### Work Done

On the second day, the focus shifted to analyzing booking trends across different months. A line chart was created to visualize booking volume over time and identify seasonal patterns.

This analysis helped understand which months experience high hotel demand and which months show lower occupancy trends.

### Key Activities

* Grouped bookings by month
* Calculated booking counts
* Created a monthly trend visualization
* Studied seasonal demand behavior

### Insights

* Peak booking months showed significantly higher demand
* Some months had lower occupancy levels
* Clear seasonal booking patterns were identified

### Code

```python
import matplotlib.pyplot as plt

# Monthly booking count
monthly_bookings = df.groupby('arrival_date_month').size()

# Plot
plt.figure(figsize=(10,5))
monthly_bookings.plot(marker='o')

plt.title("Monthly Booking Trend")
plt.xlabel("Month")
plt.ylabel("Number of Bookings")
plt.xticks(rotation=45)

plt.show()
```

---

# Day 3 – Cancellation Rate Analysis

### Work Done

The third day focused on understanding hotel booking cancellations. Monthly cancellation trends were analyzed to determine periods with high cancellation risk.

This analysis helped identify how customer cancellation behavior changes across seasons.

### Key Activities

* Filtered cancelled bookings
* Calculated monthly cancellation counts
* Compared booking and cancellation trends
* Visualized cancellation behavior

### Insights

* Certain months had higher cancellation rates
* Cancellation behavior varied seasonally
* High-demand periods also showed cancellation fluctuations

### Code

```python
# Filter cancelled bookings
cancelled = df[df['is_canceled'] == 1]

# Monthly cancellations
monthly_cancel = cancelled.groupby('arrival_date_month').size()

# Plot
plt.figure(figsize=(10,5))
monthly_cancel.plot(color='red', marker='o')

plt.title("Monthly Cancellation Trend")
plt.xlabel("Month")
plt.ylabel("Number of Cancellations")
plt.xticks(rotation=45)

plt.show()
```

---

# Day 4 – ADR (Average Daily Rate) Analysis

### Work Done

The fourth day involved analyzing ADR (Average Daily Rate) trends across different months to study seasonal pricing behavior.

This helped understand how hotel prices fluctuate depending on customer demand.

### Key Activities

* Calculated average ADR values
* Compared ADR across months
* Created seasonal pricing visualization
* Studied relationship between demand and pricing

### Insights

* ADR increased during peak booking periods
* Lower-demand months had lower pricing
* Dynamic pricing patterns were observed

### Code

```python
# Average ADR by month
monthly_adr = df.groupby('arrival_date_month')['adr'].mean()

# Plot
plt.figure(figsize=(10,5))
monthly_adr.plot(marker='o')

plt.title("Monthly ADR Trend")
plt.xlabel("Month")
plt.ylabel("Average Daily Rate")
plt.xticks(rotation=45)

plt.show()
```

---

# Day 5 – Lead Time Distribution Analysis

### Work Done

The fifth day focused on analyzing booking lead time to understand customer reservation behavior.

A density distribution plot was created to study whether customers book hotels in advance or make last-minute reservations.

### Key Activities

* Analyzed lead time feature
* Created density distribution plot
* Studied booking behavior patterns
* Identified common booking windows

### Insights

* Many customers booked within specific lead-time ranges
* Both early and last-minute booking behaviors were observed
* Booking patterns provided useful demand insights

### Code

```python
import seaborn as sns

# Lead time distribution
plt.figure(figsize=(10,5))

sns.kdeplot(df['lead_time'], fill=True)

plt.title("Lead Time Density Distribution")
plt.xlabel("Lead Time")
plt.ylabel("Density")

plt.show()
```

---

# Day 6 – Summary of EDA Findings

### Work Done

The sixth day was used to summarize all findings from the exploratory analysis and connect them with business understanding.

All visualizations and insights were reviewed to identify major customer behavior patterns and seasonal trends.

### Key Findings

* Hotel demand changes seasonally
* Peak months experience higher ADR values
* Cancellation behavior varies across months
* Customer booking behavior differs based on lead time
* Visual analysis revealed important operational insights

### Business Impact

The EDA findings can help in:

* Revenue optimization
* Better pricing strategies
* Occupancy forecasting
* Customer behavior analysis
* Business decision-making

---

# Tools & Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# Conclusion

During Week 2, Exploratory Data Analysis was performed on the hotel booking dataset to uncover patterns related to customer behavior, booking trends, cancellations, and pricing seasonality.

The analysis provided valuable insights into how hotel demand changes over time and how different factors influence hotel operations. These findings can further support predictive modeling and business strategy development.
