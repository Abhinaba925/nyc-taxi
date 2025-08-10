🎯 Project Goal
The primary objective is to build a regression model that accurately predicts the duration of a taxi trip based on pickup/dropoff coordinates, timestamps, and other trip-related metadata. The performance is evaluated using the Root Mean Squared Logarithmic Error (RMSLE).

💻 Technologies Used
This project is built entirely in Python and utilizes the following core libraries:

Data Manipulation & Analysis:

pandas

numpy

Machine Learning Models:

scikit-learn (for data splitting and metrics)

xgboost

lightgbm

catboost

Data Visualization:

matplotlib

seaborn

🔬 Methodology
The project follows a structured machine learning workflow:

1. Exploratory Data Analysis (EDA)

Before modeling, a thorough EDA was conducted to understand the data's underlying patterns. Key findings include:

The target variable, trip_duration, is highly right-skewed and benefits significantly from a log transformation.

Trip durations show clear patterns based on the hour of the day (rush hour peaks) and the day of the week (weekdays vs. weekends).

The geographical distribution of pickups is heavily concentrated in Manhattan.

2. Feature Engineering

This was the most critical step for improving model performance. The following features were created:

Haversine Distance: Calculated the great-circle distance between pickup and dropoff coordinates to get a direct measure of trip length.

Time-Based Features: Extracted the hour, day of the week, and month from the pickup_datetime.

Geospatial Features (Advanced): (Optional, but can be added) Clustering coordinates to create features for popular locations like airports (JFK, LaGuardia) or boroughs.

3. Modeling

Three powerful gradient boosting models were trained and compared:

XGBoost: A robust and widely-used library known for its performance.

LightGBM: A faster, more memory-efficient implementation of gradient boosting.

CatBoost: A model that excels at handling categorical features automatically and often yields excellent results with minimal tuning.

4. Ensembling

To maximize predictive power, the predictions from all three models were combined using a simple but effective averaging ensemble. This approach leverages the diverse strengths of each model to produce a more robust final prediction.
