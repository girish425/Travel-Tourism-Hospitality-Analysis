# Person 3 — Feature Engineering & Documentation
## 📄 Description of Work

My role was to perform feature engineering on the cleaned hotel bookings dataset and document the steps clearly. Feature engineering was done to create meaningful variables that enhance data understanding and support further analysis and machine learning tasks.

## 📂 Dataset Used
Input Dataset: cleaned_step2.csv
Output Dataset: final_cleaned_hotel_bookings.csv
## ⚙️ Feature Engineering Steps
1️⃣ Load the Dataset

The cleaned dataset obtained from the previous preprocessing step was loaded using Pandas.

import pandas as pd
import numpy as np
df = pd.read_csv('../data/cleaned/cleaned_step2.csv')

2️⃣ Create Total Stay Feature

A new feature named total_stay was created by adding the number of weekend nights and weekday nights.

df['total_stay'] = df['stays_in_weekend_nights'] + df['stays_in_week_nights']

Purpose:
Represents the complete duration of stay for each booking.

3️⃣ Create Total Guests Feature

The total_guests feature was created by summing the number of adults, children, and babies.

df['total_guests'] = df['adults'] + df['children'] + df['babies']

Purpose:
Helps analyze booking size and guest composition.

4️⃣ Create Booking Type Feature

Bookings were categorized based on lead time into:

Early Booking (lead time greater than 30 days)
Last Minute Booking (lead time 30 days or less)
df['booking_type'] = np.where(
    df['lead_time'] > 30,
    'Early Booking',
    'Last Minute'
)

Purpose:
Supports analysis of customer booking behavior.

5️⃣ Create Season Feature

A season column was created based on the arrival month of each booking.

def get_season(month):
    if month in ['December', 'January', 'February']:
        return 'Winter'
    elif month in ['March', 'April', 'May']:
        return 'Summer'
    elif month in ['June', 'July', 'August']:
        return 'Monsoon'
    else:
        return 'Autumn'

df['season'] = df['arrival_date_month'].apply(get_season)

Purpose:
Enables seasonal trend analysis in hotel bookings.

## 🔍 Final Dataset Verification

The dataset was checked to ensure all new features were added correctly and no inconsistencies were introduced.

df.head()
df.info()
## 💾 Save Final Cleaned Dataset

The final dataset with engineered features was saved for further analysis and modeling.

df.to_csv('../data/cleaned/final_cleaned_hotel_bookings.csv', index=False)
## 📊 Key Observations
Feature engineering significantly enhanced the analytical quality of the dataset.
Booking behavior can now be analyzed using stay duration, guest count, booking type, and season.
The dataset is well-structured and ready for machine learning tasks.
## 📝 Documentation Work
Added markdown explanations in the notebook
Clearly described newly created features
Updated the project README with detailed documentation
✅ Deliverables Completed

✔ New features created
✔ Final cleaned dataset prepared
✔ Documentation added
✔ README updated
