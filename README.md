# Abalone Age Prediction Analysis

## Project Overview
This project analyzes the Abalone dataset to predict the age of abalone (measured by the number of rings) using various physical measurements. Linear regression is used as the prediction model, with comprehensive evaluation of results.

## Dataset Description
The dataset contains measurements of abalone specimens with the following features:
- Sex (M: male, F: female, I: infant)
- Length (longest shell measurement)
- Diameter (perpendicular to length)
- Height (with meat in shell)
- Whole weight (entire abalone)
- Shucked weight (weight of meat)
- Viscera weight (gut weight after bleeding)
- Shell weight (after being dried)
- Rings (target variable: +1.5 gives the age in years)

## Analysis Steps

### 1. Data Visualization
- Created a correlation matrix heatmap to identify relationships between variables
- Generated scatter plots of each feature against the target variable (Rings)

### 2. Data Preparation
- Split the dataset into 80% training and 20% testing sets
- Encoded categorical 'Sex' variable using one-hot encoding

### 3. Model Training
- Trained a linear regression model using statsmodels OLS
- Examined model coefficients, standard errors, t-values, and p-values

### 4. Prediction
- Used the trained model to predict abalone age on the test dataset
- Visualized bias and variance through a residuals vs. predicted values plot

### 5. Model Evaluation
- Calculated key performance metrics:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - R-squared (R²)

### 6. Results Interpretation
- Created actual vs. predicted plots to visualize model performance
- Analyzed residuals distribution to assess model fit
- Provided interpretation of model performance and limitations

## Key Findings
- The linear regression model shows moderate predictive capability for abalone age
- Physical measurements such as shell weight and diameter show stronger correlation with age
- The model explains approximately 50-60% of the variance in abalone age (based on R² values)

## Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels

## Usage
Run the Jupyter notebook or Python script sequentially to reproduce the analysis. The code is organized by tasks, each addressing a specific aspect of the analysis pipeline.
