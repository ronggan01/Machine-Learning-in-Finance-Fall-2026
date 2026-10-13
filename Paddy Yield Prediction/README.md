# Paddy Yield Prediction

## Overview

This project predicts paddy yield using machine learning models as part of **IE 498: Machine Learning in Finance (Fall 2026)** at the University of Illinois Urbana-Champaign.

The project explores the dataset, preprocesses the features, applies dimensionality reduction using Principal Component Analysis (PCA), and compares the predictive performance of four regression models.

## Repository Contents

* `IE498_F26_Rong_Gan_project.pdf`: project report, including exploratory data analysis, methodology, model comparison, and conclusions.
* `ML_project_paddy_yield.ipynb`: Jupyter Notebook containing the data analysis, preprocessing, model training, hyperparameter tuning, and evaluation.
* `paddy_dataset.csv`: Dataset used for paddy yield prediction, obtained from the UCI Machine Learning Repository. DOI: 10.24432/C55W3J.
* `README.md`: Project overview and documentation.

## Dataset

The dataset contains **2,789 observations and 44 features**, covering agricultural and environmental factors related to paddy cultivation. The target variable is `Paddy yield(in Kg)`.


## Methodology

The project follows these steps:

1. **Exploratory Data Analysis (EDA):** Examine feature distributions, correlations, and relationships with the target variable.
2. **Preprocessing:** Split the data into training and testing sets, standardize numerical features, and one-hot encode categorical features.
3. **Dimensionality Reduction:** Apply PCA to retain at least 95% of the variance in the training predictors.
4. **Model Training and Hyperparameter Tuning:** Train and evaluate four regression models, with and without PCA:
   * Linear Regression
   * Lasso Regression
   * Random Forest
   * Support Vector Regression (SVR)
5. **Model Evaluation:** Compare models using Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), $R^2$, and training time.

## Results

SVR without PCA achieved the lowest RMSE and highest $R^2$. All eight model configurations achieved $R^2$ values between 0.9875 and 0.9907. 

For detailed results and discussion, please refer to `IE498_F26_Rong_Gan_project.pdf`.


## Author

**Rong Gan**
M.S. in Financial Engineering
University of Illinois Urbana-Champaign

## Course

IE 498 — Machine Learning in Finance, Fall 2026

