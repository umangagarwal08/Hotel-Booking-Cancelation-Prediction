# Hotel Cancellation Prediction

This repository contains the code for predicting hotel booking cancellations. The goal of this project is to analyze the data, preprocess it, build a predictive model, and deploy the model to predict the likelihood of a booking cancellation. 

## Project Workflow

### 1. Exploratory Data Analysis (EDA)
- **Visualization**: We start by analyzing the data using Matplotlib to create visualizations that provide insights into booking patterns, cancellation rates, and correlations between various features.
- **Outlier Detection**: Box plots and other methods are used to identify and treat outliers in the data.
- **Null Handling**: Null columns are dropped, and missing values are treated appropriately.

### 2. Inferential Statistics
- **Mann-Whitney U Test**: A non-parametric statistical test is applied to check for significant differences between independent variables.
  
### 3. Feature Engineering
- Features are engineered to improve model performance by creating new attributes, handling categorical data, and normalizing or scaling numerical values as needed.

### 4. Predictive Modeling
- Several classification models are built and evaluated, including:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - XGBoost
  - Ada Boost
  - Naive Bayes
  - **Gradient Boosting (Best Model)**

- A **scorecard** is generated to compare model performance based on metrics like accuracy, precision, recall, and F1-score.

### 5. Model Tuning
- **Gradient Boosting** is selected as the best model after the initial comparison.
- The model is fine-tuned using hyperparameter optimization to further improve its performance.
- The final model is saved using the **Pickle** library for later use.

### 6. Deployment
- In the deployment phase, the saved Gradient Boosting model is loaded.
- A simple local interface is created using **Gradio**, where users can input booking details and predict the likelihood of cancellation.

## Requirements

- Python 3.7 or above
- Jupyter Notebook
- Pandas
- Scikit-learn
- Matplotlib
- Gradio
- Pickle

## Results

- **Gradient Boosting** is identified as the best-performing model with fine-tuned hyperparameters.
- The final model achieves high accuracy and recall in predicting cancellations, making it suitable for deployment.
- A user-friendly interface using Gradio allows for real-time predictions.


