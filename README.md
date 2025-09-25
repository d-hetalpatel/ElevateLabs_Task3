# ElevateLabs_Task3
Implementing Linear Regression as part of internship by Elevate Labs
# House Price Prediction Using Linear Regression

This project demonstrates how to predict house prices using linear regression with both numerical and categorical features. It includes data preprocessing, model training, evaluation, and interpretation of results.

## Dataset
The dataset contains the following columns:

- price
- area
- bedrooms
- bathrooms
- stories
- parking
- mainroad
- guestroom
- basement
- hotwaterheating
- airconditioning
- prefarea
- furnishingstatus

## Features
- **Numerical features:** area, bedrooms, bathrooms, stories, parking  
- **Categorical features:** mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus  

## Steps
1. Load the dataset using pandas.
2. Separate numerical and categorical features.
3. One-hot encode categorical features.
4. Combine numerical and encoded categorical features.
5. Split the data into training and testing sets.
6. Train a linear regression model.
7. Predict on the test set.
8. Evaluate model performance using MSE, MAE, and R² score.
9. Interpret model coefficients.

## Evaluation Metrics
- **Mean Squared Error (MSE):** Measures average squared difference between actual and predicted values. Penalizes large errors more.
- **Mean Absolute Error (MAE):** Measures average absolute difference between actual and predicted values. Robust to outliers.
- **R² Score:** Indicates how much variance in the target variable is explained by the model. Ranges from 0 to 1.

## Assumptions of Linear Regression
- Relationship between features and target is linear
- Observations are independent
- Errors have constant variance
- Errors are normally distributed
- Features are not highly correlated
- Errors are not autocorrelated

## Interpreting Coefficients
- Each coefficient shows how the target changes if the feature increases by one unit, keeping others constant
- Positive coefficient: target increases
- Negative coefficient: target decreases
- For categorical features, the coefficient shows effect relative to the baseline category

## Limitations
- Cannot handle non-linear relationships unless features are transformed
- Sensitive to outliers
- Cannot be used directly for classification tasks

## How to Run
1. Clone the repository.
2. Place your dataset CSV file in the project folder (e.g., `house_price.csv`).
3. Run the Python script:

```bash
python house_price_lr.py
