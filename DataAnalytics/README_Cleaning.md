# Data Cleaning 

# Project Overview
This project focuses on cleaning and preparing raw customer behavioral data for machine learning models. 
It transforms messy transactional data into a sanitized dataset by addressing data quality issues, handling structural anomalies, and applying statistical capping methods.

## Data Cleaning Steps
Data Sanitization: Removed duplicate rows and imputed/removed missing values to ensure data integrity.
Format & Type Casting: Converted raw dates into explicit `datetime64` objects and cast transactional metrics into numeric types.
Outlier Capping (IQR Method): Used the Interquartile Range method ($Q3 + 1.5 \times IQR$) to cap extreme values in spend and purchase volumes without discarding records.
Feature Normalization: Standardized numerical variables using `StandardScaler` to ensure uniform feature scaling.

# Tech Stack
Language: Python
Libraries: Pandas, NumPy, Seaborn, Metplotlib
