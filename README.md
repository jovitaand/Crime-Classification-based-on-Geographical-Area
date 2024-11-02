# Crime Classification Based on Geographical Area

## Overview

This project aims to develop a system for crime classification based on geographical areas, using data-driven techniques to understand crime patterns. The system provides insights into crime occurrences in specific neighborhoods, making it a valuable resource for real estate agents, residents, and law enforcement agencies to assess safety and make informed decisions.

## Team Members
- Navya Kiran V B
- Madhumitha Saravanan
- Sindhuja Maheswaran
- Jovita Andrews
- Spruha Chandrakant Band

## Objective

The main goal of this project is to classify and analyze crimes based on their geographical location. By identifying crime patterns and trends in different neighborhoods, the system helps users make data-driven decisions about safety. The project empowers stakeholders with insights on crime statistics to optimize safety measures and strategies in particular areas.

## Data Sources

The data for this project was sourced from:
- **Los Angeles Police Department (LAPD)**: A dataset containing detailed information on reported crimes, including location, time, type of crime, and victim details.

## Data Preparation and Cleaning

The following steps were taken to ensure data reliability and usability:
- **Column Renaming**: Cryptic column names were renamed for better readability.
- **Handling Missing Values**: Various techniques, such as mode imputation for categorical data and mean/median imputation for numerical data, were used to fill missing values.
- **Outlier Handling**: Outliers, especially in victim age data, were identified and addressed using statistical techniques like the Interquartile Range (IQR) method.

## Feature Engineering

Several new features were engineered to enhance analysis:
- **Crime Severity**: Crimes were categorized based on their impact, e.g., homicides were classified as high-severity, while petty theft was classified as low-severity.
- **Victim Demographics**: Features representing victim age, gender, and ethnicity were created to better understand crime susceptibility across different demographic groups.

## Exploratory Data Analysis (EDA)

Key analyses include:
- **Location-Based Heatmaps**: Heatmaps were created to visualize areas with high crime concentrations.
- **Demographic Analysis**: Crime reports were analyzed across different demographic categories like age, gender, and ethnicity.
- **Time Series Analysis**: Temporal trends in crime occurrences were examined, identifying peak times for crimes such as higher incidents on Fridays and during the month of July.

## Methods

Various machine learning classifiers were used, including:
- **Random Forest Classifier**
- **XGBoost Classifier**
- **Logistic Regression**
- **Recurrent Neural Network (RNN)**

### Synthetic Minority Over-sampling Technique (SMOTE)

SMOTE was applied to balance class distribution in the dataset, particularly addressing underrepresented classes. This helped improve model performance by mitigating issues of class imbalance.

### Model Evaluation

- **Random Forest (pre-SMOTE)**: Achieved 75% accuracy with a recall of 0.90 for the majority class.
- **XGBoost (pre-SMOTE)**: Achieved 72.8% accuracy.
- **Post-SMOTE Models**: Both Random Forest and XGBoost models saw a slight accuracy drop to 68%, balancing class distribution.
- **Logistic Regression**: Maintained an accuracy of 72%.
- **SimpleRNN Model**: Achieved a test accuracy of 50.62%.

## Results

The analysis revealed significant crime patterns, such as:
- Higher crime occurrences in single-family dwellings and streets.
- Victim demographics show that individuals in their late teens to early thirties are most frequently targeted.
- Geographic areas with the highest concentrations of crime were identified, assisting in targeted safety measures.

## Conclusion and Future Scope

The system has the potential to significantly improve safety awareness and decision-making for various users, including real estate agents and residents. Future work may involve expanding the data sources, refining machine learning models, and improving the user interface to provide more detailed and accessible insights.


 

