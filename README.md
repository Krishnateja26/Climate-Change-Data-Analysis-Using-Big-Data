# Climate-Change-Data-Analysis-Using-Big-Data

# Climate Change Data Analysis Using Big Data

## Presented By
- **Krishna Teja Reddy Suram**
- **LakshmiPriya Palaparthy**

---

## Table of Contents

1. [Introduction](#introduction)
2. [Business Problem](#business-problem)
3. [Data Sources](#data-sources)
4. [Data Understanding](#data-understanding)
5. [Data Visualization](#data-visualization)
6. [Model Building](#model-building)
7. [Conclusion](#conclusion)
8. [Future Work](#future-work)

---

## 1. Introduction

### Project Significance
Understanding weather patterns and severe weather events is crucial in today's climate-conscious society. This project enhances climate resilience by analyzing large-scale U.S. weather data to identify patterns that help predict extreme events and support disaster preparedness. Leveraging big data tools like Apache Spark on Databricks, the project provides crucial insights for data-driven climate research and mitigation strategies, aiding communities and policymakers in making informed decisions.

### Methodology Overview
- **Tools Used:** PySpark on Databricks
- **Key Steps:**
  - Data preprocessing and cleaning
  - Missing data handling
  - Temporal-spatial analysis for weather patterns
  - Machine learning models for event prediction

---

## 2. Business Problem

### Problem Statement
This project aims to generate actionable insights into weather trends using big data analytics. The goal is to identify patterns and predict extreme events, providing valuable resources for researchers, meteorologists, and policymakers to support data-driven decisions. These insights enhance climate resilience and community preparedness against evolving weather patterns.

### Challenges
- Increasing frequency and intensity of extreme weather events like hurricanes and heatwaves.
- Lack of timely warnings and localized weather information, leaving communities unprepared.
- Exacerbated risks due to climate change, making it harder to protect lives and property.

---

## 3. Data Sources

### Dataset Overview
- **Scope:** Covers weather events across 49 U.S. states.
- **Number of Events:** 8.6 million
- **Weather Types:** Regular occurrences (e.g., rain, snow) and extreme events (e.g., storms, freezing conditions).
- **Time Span:** January 2006 to December 2016
- **Data Sources:** 2,071 airport-based weather stations nationwide
- **Dataset Size:** 1.1 GB

---

## 4. Data Understanding

### Key Variables
1. **Formatted Date:** Timestamps with timezone information
2. **Summary:** Brief weather descriptions
3. **Precip Type:** Type of precipitation (e.g., rain)
4. **Temperature (C):** Actual temperature in Celsius
5. **Apparent Temperature (C):** "Feels like" temperature in Celsius
6. **Humidity:** Relative humidity (0-1)
7. **Wind Speed (km/h):** Wind speed
8. **Wind Bearing (degrees):** Wind direction in degrees
9. **Visibility (km):** Distance of visibility in kilometers
10. **Cloud Cover:** Cloud coverage
11. **Pressure (millibars):** Atmospheric pressure
12. **Daily Summary:** Detailed weather summaries

### Dataset Cleaning
- **Date Formatting:** Standardized date field for consistency.
- **Null Value Handling:** Removed null values to improve reliability.
- **Duplicate Removal:** Ensured unique data points to avoid bias.

---

## 5. Data Visualization

### Key Visualizations
1. **Temperature Over Time:** Seasonal variations with peaks in warmer months and dips in colder months.
2. **Precipitation Counts:** Rain dominates the dataset, with significantly fewer snow events.
3. **Pressure Over Time:** Stable readings with occasional anomalies, requiring further investigation.
4. **Wind Speed vs. Wind Bearing:** Uniform distribution across wind bearings with most speeds below 20 km/h.
5. **Humidity Distribution:** Predominantly high humidity values, clustering between 0.8 and 1.
6. **Wind Speed Over Time:** Consistent variability with occasional high-wind events.
7. **Temperature vs. Humidity:** Inverse relationship between temperature and humidity.

---

## 6. Model Building

### 1. Linear Regression (PySpark)
- **Objective:** Predict Apparent Temperature (C) based on weather features.
- **Key Metrics:**
  - **MSE:** 1.174
  - **R²:** 0.9897
- **Insights:** Strong predictive accuracy with 98.97% of variance explained by features.

### 2. Random Forest Classification
- **Objective:** Predict precipitation types (rain, snow, or none).
- **Key Metrics:**
  - **Precision:** 99.51%
  - **Recall:** 99.59%
  - **F1-Score:** 99.48%
- **Feature Importances:**
  - **Wind Speed:** 0.92
  - **Cloud Cover:** 0.03

### 3. Logistic Regression
- **Objective:** Classify severe vs. non-severe weather events.
- **Key Metrics:**
  - **Accuracy:** 0.9926
  - **Precision:** 0.9926
  - **Recall:** 0.9926
  - **AUC:** 0.9905
- **Confusion Matrix:**
  - **TP:** 1169 | **TN:** 18014
  - **FP:** 64 | **FN:** 79

---

## 7. Conclusion

### Summary of Achievements
1. **Regression Model:** Predicted apparent temperature with high accuracy.
2. **Random Forest Model:** Accurately classified precipitation types.
3. **Logistic Regression Model:** Identified severe weather events with strong performance metrics.

These insights, powered by Databricks and big data tools, provide valuable resources for understanding and predicting weather trends, supporting better decision-making for climate resilience.

---

## 8. Future Work

### Proposed Enhancements
1. **Real-Time Prediction:**
   - Integrate models into real-time forecasting systems using Apache Kafka with Spark.
2. **Expanding the Dataset:**
   - Include global weather data for broader trends and recent data for up-to-date predictions.
3. **Enhancing Feature Engineering:**
   - Add seasonal trends and geographical data to improve model performance.
   - Explore derived features like temperature fluctuations and advanced weather indices.

---

## Thank You!
### Questions?
Feel free to reach out for further clarifications or discussions!
