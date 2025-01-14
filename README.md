# Property Listings Analysis and Price Prediction

## Overview

This project focuses on analyzing property listing data to understand trends and build a regression model to predict property prices. The dataset contains detailed information about property listings, such as host attributes, listing details, and customer reviews. Through exploratory data analysis (EDA) and regression modeling, we aim to uncover insights and predict property prices based on various features.

## Objectives

- Perform exploratory data analysis (EDA) to understand the dataset and uncover trends.
- Identify multicollinearity using Variance Inflation Factor (VIF).
- Build regression models to predict property prices.
- Evaluate model performance using metrics such as Root Mean Squared Error (RMSE).

## Dataset Details

The dataset includes the following key columns:

- **id**: Unique identifier for each listing.
- **host_id**: Unique identifier for each host.
- **host_response_time**: Host response time to inquiries.
- **host_response_rate**: Percentage of inquiries the host responds to.
- **review_scores_value**: Review scores based on customer feedback.
- **cancellation_policy**: Cancellation policy for the listing.
- **price**: Target variable representing the listing price.
- **reviews_per_month**: Average number of reviews received monthly.

## Key Steps

### 1. Exploratory Data Analysis (EDA)

- Understand the distribution and characteristics of the data.
- Visualize key variables to identify trends and outliers.

### 2. Data Cleaning

- Handle missing values in columns such as `host_response_rate` and `reviews_per_month`.
- Convert categorical values (`t`, `f`) to boolean (`True`, `False`).

### 3. Multicollinearity Check

- Use the Variance Inflation Factor (VIF) to identify highly correlated variables.
- Drop variables with high VIF to reduce multicollinearity and improve model performance.

### 4. Regression Modeling

- Build regression models to predict `price` using relevant features.
- Evaluate model performance using RMSE on training and test datasets.

### 5. Results Evaluation

- Compare RMSE values for different models to determine the best approach.
- Interpret the coefficients to understand the impact of features on price.

## Model Performance

- **RMSE on Training Set**:
  - Model 1: 24.45
  - Model 2: 24.45

- **RMSE on Test Set**:
  - Model 1: 23.84
  - Model 2: 23.84

The close RMSE values between training and test sets indicate good generalization by the models.

## Tools and Libraries

- **Python Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Statsmodels, Scikit-learn.
- **Visualization Tools**: Seaborn and Matplotlib for EDA.
- **Mapping**: Folium library for geospatial visualization (if applicable).

## Conclusion

This project demonstrates the application of regression modeling to predict property prices. By analyzing the dataset, addressing multicollinearity, and evaluating model performance, we gain valuable insights into the factors influencing property prices.

## Future Work

- Enhance the model with advanced algorithms (e.g., Random Forest, Gradient Boosting).
- Incorporate geospatial analysis to understand the impact of location.
- Use hyperparameter tuning to further optimize the regression models.


## Instructions to Run

1. Install the required Python libraries:
   ```bash
   pip install pandas numpy seaborn matplotlib statsmodels scikit-learn folium
