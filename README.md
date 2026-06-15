**Overview**
This project explores the relationship between climate conditions, air quality, socioeconomic factors, and respiratory disease rates using a global dataset covering approximately 14,000 weekly observations from 2015–2025.
The goal was to determine which environmental and socioeconomic factors are most strongly associated with respiratory disease rates and whether these variables can be used to predict respiratory health outcomes across countries.

**Research Questions**
How strongly do climate factors predict respiratory disease rates?
Does air quality have a larger impact than weather conditions?
Do socioeconomic factors improve predictive performance?
Which variables contribute most to respiratory disease predictions?
Which countries and regions experience the highest respiratory disease burden?

**Dataset**
Source: Kaggle
The dataset contains weekly observations from countries around the world and includes:
Climate Variables
Temperature
Precipitation
Heatwave indicators
Flood indicators
Drought indicators
Air Quality Variables
Air Quality Index (AQI)
Socioeconomic Variables
Income level
GDP per capita
Healthcare access index
Food security index
Mental health index
Health Outcomes
Respiratory disease rate

**Methods**
Data Preparation
Cleaned and processed weekly observations
Encoded categorical variables
Standardized continuous predictors using StandardScaler
Split data into training and testing sets
Modeling
Linear Regression
Feature importance analysis using standardized coefficients
Model evaluation using:
R² Score
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Exploratory Analysis
Country-level comparisons
Regional comparisons
Correlation analysis
Variable importance visualization

**Key Findings**
Air Quality Was the Strongest Predictor
Air Quality Index (AQI) consistently produced the largest contribution to model performance.
Models including AQI substantially outperformed models using weather variables alone.
Weather Alone Had Limited Predictive Power
Removing AQI caused model performance to drop significantly.
Temperature, precipitation, and extreme weather indicators explained only a small portion of respiratory disease variation by themselves.
Socioeconomic Variables Added Little Predictive Power
Adding income, healthcare access, and related indicators did not meaningfully increase R².
This suggests that much of their influence is already reflected through air quality measures or long-term structural differences between countries.
Lower-Income Countries Experienced Higher Disease Burdens
Country-level analysis showed that many countries with the highest respiratory disease rates also had:
Higher air pollution levels
Lower income classifications
Lower healthcare access measures

**Example Visualizations**
Project outputs include:
Actual vs Predicted respiratory disease rates
Variable importance plots
Country-level respiratory disease rankings
Regional comparisons
Climate vs health relationship visualizations

**Technologies Used**
Python
Pandas
NumPy
Matplotlib
Scikit-Learn

**Skills Demonstrated**
Data Cleaning
Exploratory Data Analysis (EDA)
Feature Engineering
Linear Regression
Model Evaluation
Data Visualization
Public Health Data Analysis
Environmental Data Analysis

**Future Improvements**
Potential extensions include:
Random Forest and XGBoost models
Time-series forecasting methods
Country fixed-effects models
Causal inference approaches
Additional environmental indicators such as PM2.5 and humidity

**Takeaway**
The analysis suggests that air quality plays a much larger role in short-term respiratory disease outcomes than general weather conditions. While climate and socioeconomic factors remain important, air pollution emerged as the most consistent predictor of respiratory health across the dataset.

