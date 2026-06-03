# NYC-Motor-Vehicle-Collisions-Analyzing-Crashing-Severity-From-Police-Data-

This project analyzes over 470,000 NYC motor vehicle collision records to predict crash severity using classification models in R. The dataset spans January 2020 through December 2024 and was sourced from the NYC Open Data portal.

Following extensive data cleaning, reverse geocoding to fill missing location data, and feature engineering, crashes were labeled into three severity classes: Low, Moderate, and High, based on injuries and fatalities. With only 1.2% of crashes classified as High severity, stratified undersampling was applied to balance the classes before modeling.

Four modeling approaches were evaluated including kNN, Gradient Boosting, Decision Tree (C5.0 and rpart), and Random Forest. The C5.0 decision tree was the top performer, with 71% sensitivity for High severity crashes, meaning it was reasonably effective at identifying the most serious collisions. The most influential predictors were vehicle type, contributing factor, crash datetime, and borough.

While the models had room for improvement in distinguishing between severity classes, exploratory analysis revealed meaningful patterns. Collisions peak on Fridays and during afternoon hours, Brooklyn has the highest crash volume, and unsafe driving(particularly texting while driving) is the dominant contributing factor. Future improvements would benefit from richer feature sets such as weather conditions and road type.
