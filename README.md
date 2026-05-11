# Used Car Price Prediction using Machine Learning

## Project Overview:
                  This project focuses on predicting used car prices using multiple Machine Learning regression algorithms. The complete ML pipeline includes data preprocessing, feature engineering, feature scaling, regularization techniques, ensemble learning, hyperparameter tuning, and model evaluation.

## Goal:
     The objective was to compare different regression models and identify the best-performing model for accurate car price prediction.
## Project Workflow

### Data Preprocessing
         Removed unnecessary columns
         Handled duplicate records
         Identified suspicious outliers using domain knowledge
         Applied log transformation on target variable (selling_price) to reduce skewness
         
### Feature Engineering
         Performed One-Hot Encoding on categorical features
         Explored feature cardinality (brand, model, car_name)
         Compared different feature selection strategies:
             Brand only
             Model only
             Car Name
             Brand + Model
             
### Feature Scaling
      Used StandardScaler for scale-sensitive models:
      Linear Regression, Ridge Regression, Lasso Regression

    (Tree-based models like Random Forest and XGBoost were trained without scaling.)

## Models Implemented:

🔹 Linear Regression

Baseline regression model.

🔹 Ridge Regression

Applied L2 Regularization to reduce the impact of multicollinearity and stabilize coefficients.

🔹 Lasso Regression

Applied L1 Regularization for feature shrinkage and feature selection analysis.

🔹 Random Forest Regressor

Ensemble tree-based model capable of capturing non-linear relationships.

🔹 XGBoost Regressor

Boosting-based ensemble model that achieved the best performance.
     

## Hyperparameter Tuning:
                  -> RidgeCV
                  -> LassoCV
                  -> RandomizedSearchCV
