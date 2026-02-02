## Simple Linear Regression Lab: Fuel Consumption & Emissions Analysis

## 📊 Project Overview

This hands-on lab demonstrates the implementation of Simple Linear Regression to predict CO₂ emissions from vehicles based on fuel consumption and engine characteristics. Using Python's scikit-learn library, the project walks through the complete machine learning workflow: data exploration, train/test splitting, model training, prediction, and evaluation using multiple statistical metrics.

## 📁 Dataset Description

a. Source: Fuel Consumption Ratings dataset (Environment Canada)

b. Features:

- ENGINESIZE: Engine size in liters
- CYLINDERS: Number of cylinders
- FUELCONSUMPTION_CITY: Fuel consumption in city (L/100 km)
- FUELCONSUMPTION_HWY: Fuel consumption on highway (L/100 km)
- FUELCONSUMPTION_COMB: Combined fuel consumption (L/100 km)
- FUELCONSUMPTION_COMB_MPG: Combined fuel consumption (miles per gallon)
- CO2EMISSIONS: CO₂ emissions in grams per kilometer (target variable)

c. Dataset Characteristics:

- 1,067 vehicle records
- Numerical features suitable for regression analysis
- Clean dataset with no missing values

## 🎯 Learning Objectives

By completing this lab, you will learn to:

- Perform exploratory data analysis (EDA) using scatter plots
- Split datasets into training and testing subsets
- Train a simple linear regression model using scikit-learn
- Make predictions on unseen test data
- Evaluate model performance using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R²-score (coefficient of determination)
- Compare model performance when trained on different features
- Visualize regression results to assess model fit

## ⚙️ Technical Requirements

- Python Libraries : pip install pandas numpy matplotlib scikit-learn

- Required Imports
  
  <img width="604" height="156" alt="Screenshot 2026-02-02 at 15 11 40" src="https://github.com/user-attachments/assets/7ba91df7-b421-484d-b443-03c09adaba25" />

## 🔬 Methodology
<img width="604" height="454" alt="Screenshot 2026-02-02 at 15 21 11" src="https://github.com/user-attachments/assets/ccfeff41-c6a0-47e9-b2f9-63fa253f42de" />

1. Data Exploration
   
- Visualize relationships between features and target variable using scatter plots
- Identify strong linear correlations (e.g., between FUELCONSUMPTION_COMB and CO2EMISSIONS)
  
2. Data Preparation
   <img width="604" height="173" alt="Screenshot 2026-02-02 at 15 13 00" src="https://github.com/user-attachments/assets/a7e726c4-5e8e-43f5-8862-f3d371a81ce6" />
   
3. Model Training
   <img width="604" height="173" alt="Screenshot 2026-02-02 at 15 14 49" src="https://github.com/user-attachments/assets/f9627ff5-90fb-4736-9cba-730d7cae1c6e" />


4. Prediction & Evaluation

<img width="604" height="220" alt="Screenshot 2026-02-02 at 15 15 10" src="https://github.com/user-attachments/assets/4c367f0b-0574-4da8-bc47-8e1c1b245565" />

5. Visualization

- Plot regression line over training data to visualize model fit
- Compare predictions against actual values on test data
- Assess residuals to identify prediction patterns
  
## 💡 Key Insights
### Feature Comparison:

- Models trained on FUELCONSUMPTION_COMB achieve lower MSE than those trained on ENGINESIZE
- Combined fuel consumption has stronger linear relationship with CO₂ emissions than engine size alone

### Model Interpretation:
- Positive coefficient confirms: higher fuel consumption → higher CO₂ emissions
- R²-score typically >0.85 indicates strong explanatory power of the linear model

### Practical Application:
- Simple linear regression provides interpretable relationship between fuel consumption and emissions
- Model can estimate emissions for new vehicles based on fuel efficiency ratings

## 🚀 How to Run
Download the dataset:

!wget -O FuelConsumption.csv https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork/labs/Module%202/data/FuelConsumptionCo2.csv


Execute notebook cells sequentially:

- Start with data loading and exploration
- Proceed through train/test splitting
- Train models with different features
- Evaluate and compare results

Complete practice exercises:
- Plot regression results over test data (not just training data)
- Experiment with different features (ENGINESIZE vs FUELCONSUMPTION_COMB)
- Interpret evaluation metrics in practical context

