# Boom Bikes Sharing Case Study
> Case Study of Linear Regression model for a US bike-sharing provider BoomBikes.


## Table of Contents :
* [Problem Statement]
* [Objectives]
* [Approach]
* [Conclusions]
* [Glossary]

## Problem Statement
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands.

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 
 
 ## Objectives
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 
Please find the [Bike Sharing dataset](./day.csv) here and [Data dictionary](./Data%20dictionary.txt) here.

## Approach

- Step 1: Import Necessary Libraries
- Step 2: Load the Data and Understanding the Data
- Step 3: Data Cleaning and Missing Value Check
- Step 4: Segmentation of Columns
- Step 5: Exploratory Data Analysis (EDA)
-- Univariate Analysis (One Variable at a Time)
-- Bivariate Analysis (Two Variables at a Time)
-- Multivariate Analysis (More Than Two Variables at a Time)
- Step 6: Data Preparation Steps
-- Dummy Variable Creation (One Hot Encoding)
- Step 7: Train-Test Split
- Step 8: Feature Scaling (Min-Max Scaling / Normalization)
- Step 9: Building the Initial Linear Model (Model 0)
- Step 10: Feature Selection (Using RFE and Manual Selection Methods)
- Step 11: Check and Build the Models Using Selected Features
- Step 12: Residual Analysis of the Train Data
- Step 13: Making Predictions Using the Final Linear Model
- Step 14: Steps for Further Model Refinement and Optimization
- Step 15: Model Evaluation



## Conclusions
**From the Exploratory Data Analysis , we can conclude the following -**
- Bike rental counts are lowest in spring and highest in fall, with summer showing significantly peak rentals.
- There was an increase in bike rentals in 2019 compared to 2018.
- Data for heavy_snow_rain weather situations is missing, potentially affecting analysis of extreme weather impacts.
- Bike rentals peak in June, July, and September, with lower counts in January.
- More bike rentals occur on working days compared to non-working days.
- Rental counts are higher on non-holidays compared to holidays.
- Rental demand remains consistent across all weekdays.
- Favorable weather "Clear Sky" correlates with higher rental counts, while poor weather "Light snowy rain" correlates with lower counts. There is no occurance for "Heavy snowy rain".
- Strong positive correlations exist between temperature (temp/atemp) and rental counts.
- Registered users show a strong positive correlation with rental counts.
- Casual users also positively correlate with rental counts, though less strongly than registered users.
- Humidity and windspeeds show weak correlations with rental counts and other variables.
- Humidity and windspeeds show weak correlations with rental counts and other variables.
- Bike rentals increase from March to June and decrease towards the end of the year.
- Higher temperatures (temp/atemp) positively influence rental counts.

**Q : Which variables are significant in predicting the demand for shared bikes? How Well the Significant Variables Describe Bike Demand ?**
- High R-squared: The model explains 84.48% of the variance in bike demand for the training set and 80.51% for the test set, indicating a strong fit.
- Temperature: There is a strong positive relationship, with higher temperatures significantly increasing bike demand.
- Year (2019): Shows a substantial increase in bike demand in 2019 compared to 2018, indicating a growing trend.
- Weather Conditions: Adverse weather reduces demand, especially during light snow/rain and misty conditions.
- Windspeed and Humidity: Both negatively impact demand, with higher windspeed and humidity levels leading to decreased bike usage.
- Seasonal Effects: Higher demand is observed in Fall , Summer and Winter.
- Monthly Effects: Lower demand in January and July, higher demand in September.
- Weekday Monday: Positive effect on bike demand.
- Working Day: Increases bike demand.


## Glossary

- Data Visualization
- EDA (Exploratory Data Analysis)
- Feature Scaling (Normalization)
- Dummy Variable (One Hot Encoding)
- Linear Regression
- p-value and Confidence Interval
- Coefficient of Determination (R²) and Adjusted R²
- Mean Squared Error (MSE) and Root Mean Squared Error (RMSE)
- Cross-Validation
- Multicollinearity
- Residuals Analysis

