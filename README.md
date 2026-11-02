Predictive Insight Engine :

House Price Prediction Using Regression

A machine learning project that predicts house prices using regression
algorithms. This project compares different regression models, explores
gradient descent optimization, and evaluates model performance using
regression metrics and model diagnostics.

🎥 Project Video Presentation

Watch the project presentation:
link: https://drive.google.com/file/d/11PQ88w3scR1Y6dxaQO9sLl3yvN9ldRrg/view

📌 Project Overview

The objective is to estimate house prices from property-related features
and compare different regression approaches.

This project covers: - Simple Linear Regression - Multiple Linear
Regression - Polynomial Regression (Degree 2) - Batch Gradient Descent -
Stochastic Gradient Descent (SGD) - Mini-Batch Gradient Descent - Model
evaluation and diagnostics - Bias--variance, overfitting, and
underfitting analysis

📂 Dataset

The project uses RealEstate_HousePrice_Dataset_4200.xlsx, containing
approximately 4,200 records and 12 columns.

Column                   Description

house_id               Unique house identifier
area_sqft              House area in square feet
bedrooms               Number of bedrooms
bathrooms              Number of bathrooms
location_score         Numerical location score
age_years              Age of the property
distance_city_km       Distance from the city
lot_size_sqft          Plot size in square feet
has_garage             Whether the property has a garage
has_pool               Whether the property has a pool
renovation_years_ago   Years since renovation
house_price_inr        Target house price in INR

house_id is excluded from model inputs because it is an identifier.
The target variable is house_price_inr; the remaining 10 property
features are used as predictors.

🛠️ Technologies and Libraries

Python

Pandas

NumPy

Matplotlib

Scikit-learn

Jupyter Notebook / Google Colab


⚙️ Project Workflow

Load and inspect the dataset.

Check data types, missing values, and duplicate records.

Separate input features and target variable.

Split the data into training and testing sets.

Train Simple Linear Regression.

Train Multiple Linear Regression.

Train Polynomial Regression (Degree 2) using all 10 input features.

Implement and compare Batch, Stochastic, and Mini-Batch Gradient
Descent.

Evaluate model performance.

Analyze bias, variance, overfitting, and underfitting.


🤖 Regression Models

1. Simple Linear Regression

Uses only area_sqft to model the relationship between house area and
house price.

2. Multiple Linear Regression

Uses all 10 property features to predict house prices.

3. Polynomial Regression (Degree 2)

Expands all 10 input features into degree-2 polynomial features,
including squared terms and pairwise interactions, then fits a linear
regression model to the expanded data.


📉 Gradient Descent Optimization

The project explores three optimization methods:

Batch Gradient Descent: Uses the entire training dataset for
each parameter update.

Stochastic Gradient Descent (SGD): Uses one training example for
each parameter update.

Mini-Batch Gradient Descent: Uses a small group of training
examples for each parameter update.

Scikit-learn's SGDRegressor is also used to demonstrate stochastic
optimization.

For gradient-descent experiments, features and target values are
standardized using training-set statistics. Predictions are
inverse-transformed before reporting errors in INR.


📊 Evaluation Metrics

Metric     Purpose

MAE        Average absolute prediction error
MSE        Average squared prediction error
RMSE       Square root of MSE, expressed in the target's units
R² Score   Proportion of target variation explained by the model

For regression, R² is a performance metric; it is not classification
accuracy.


📈 Visualizations and Model Diagnostics

The project includes: - R² score comparisons between regression
models. - Training-versus-testing performance comparisons. -
Actual-versus-predicted house-price plots. - Cost-versus-epoch plots for
gradient descent. - Convergence and training-time comparisons of
gradient-descent methods. - Bias--variance and overfitting/underfitting
analysis.

Overfitting and Underfitting

Underfitting: The model performs poorly on both training and
testing data.

Overfitting: The model performs very well on training data but
noticeably worse on unseen testing data.

Good generalization: The model performs well on testing data
with a reasonably small training--testing performance gap.

Training--testing gaps are useful diagnostic indicators, but they are
not direct measurements of statistical bias and variance.


🎯 Key Learning Outcomes

Understanding supervised learning and regression.

Comparing simple, multiple, and polynomial regression.

Understanding gradient descent and its variants.

Evaluating regression models with appropriate metrics.

Identifying possible overfitting and underfitting.

Understanding model complexity and the bias--variance trade-off.

🔮 Future Improvements

Use cross-validation for more reliable model comparison.

Tune model parameters and compare Ridge and Lasso regression.

Experiment with additional regression algorithms.

Add residual analysis and prediction intervals.

Deploy the selected model through a web application.
