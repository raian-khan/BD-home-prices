# House Price Prediction in Bangladesh

## Overview
This project aims to predict house prices in Bangladesh using a dataset from Kaggle (`house_price_bd.csv`) and seven different machine learning models. Despite data cleaning, feature engineering, and outlier removal, the dataset posed challenges due to its imbalance. However, **GradientBoostingRegressor** and **RandomForestRegressor** emerged as the best-performing models.

## Dataset
The dataset contains information about house prices in Bangladesh, including features like location, square footage, number of bathrooms, bedrooms, and more. The dataset is moderately clean but suffers from imbalances impacting prediction accuracy.

### Steps Taken:
1. **Data Cleaning:**
   - Handled missing values.
   - replaced unusual values with proper numerical values
   - Removed duplicate entries.

2. **Feature Engineering:**
   - One-hot encoded categorical variables (e.g., location).

3. **Outlier Removal:**
   - Identified and removed outliers based on statistical methods.

4. **Model Training:**
   - Split the data into training and testing sets.
   - Trained the models using 80% of the data and evaluated on the remaining 20%.

## Machine Learning Models
Seven machine learning models were used:

1. **LinearRegression**
2. **SVR (Support Vector Regressor)**
3. **DecisionTreeRegressor**
4. **RandomForestRegressor**
5. **KNeighborsRegressor**
6. **GradientBoostingRegressor**
7. **XGBRegressor (Extreme Gradient Boosting)**

### Evaluation Metrics:
- **Mean Squared Error (MSE):** Measures the average squared difference between predicted and actual values.
- **R² Score:** Indicates how well the model explains the variance in the data (1 is perfect, 0 is poor).

### Results:
The two best-performing models were:

1. **GradientBoostingRegressor**
   - Consistently high R² scores across training and testing data.
   - Performed well on unseen data.

2. **RandomForestRegressor**
   - Slightly less consistent than Gradient Boosting but still a top performer.

## Challenges:
- **Unbalanced Dataset:** Despite preprocessing efforts, the dataset's imbalance made achieving high accuracy in predictions difficult.
- **Moderate Dataset Quality:** Limited features and some inconsistencies impacted the predictive power.

## Future Improvements:
- Try the models on a better dataset.
- Implement hyperparameter tuning for further model optimization.
- Consider deep learning models for better feature representation and prediction.
