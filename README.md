## Project Overview
This project analyzes gym member behavior to understand churn causes and improve retention.
Objectives: Identify churn drivers and build a predictive classification model.
Dataset: Covers demographics (Age, Gender), activity (visits, membership type), and subscription status.
Key Questions: Factors causing churn, relationship between activity and retention, and impact of age/membership type.
Model Type: Classification.

## Data Cleaning
Steps taken to prepare the raw data for analysis:
Initial Cleanup: Removed non-predictive personal identifiers (Member_ID, Name, Phone, Address).
Missing Values: Imputed missing numerical values with the column mean and removed rows with missing critical dates.
Formatting: Converted date columns to datetime objects.
Deduplication: Removed duplicate entries to ensure unique records.
## Data Preprocessing

Preparation steps for machine learning:
Encoding: Converted categorical variables (Membership_Type, Favorite_Exercise) into numerical dummy variables using get_dummies (with drop_first=True to avoid redundancy).
Target Mapping: Mapped Churn labels (Yes/No) to binary values (1/0).
Feature Scaling: Applied StandardScaler to numerical features (Age, Calories, Duration, etc.) to normalize ranges for better model performance.\

## Visualization & Insights
Summary of data analysis and findings:
Demographics: Members are primarily aged 25-45; Gender distribution is balanced (51.1% Male, 48.9% Female).
Activity: Most members burn 350-620 calories per session.
Correlation Analysis: A strong negative correlation (-0.72) exists between Visits_Per_Month and Churn.
Key Finding: Higher visit frequency is the most significant indicator of member retention; low visit frequency strongly correlates with churn.


*Team Members*:
Joice mena refaat,
Zamzam Mohammed Naser,
Noura Ashraf Abuelyazed,
Malak Elhusany Abdullah,
Eman Mohamed Elbadry
