# House Prices – Advanced Regression Techniques

Predict residential home sale prices in Ames, Iowa using creative feature engineering and advanced regression models (Random Forests, Gradient Boosting, XGBoost).

---

## 📋 Table of Contents

1. [Overview](#overview)  
2. [Project Structure](#project-structure)  
3. [Getting Started](#getting-started)  
4. [Data](#data)  
5. [Methodology](#methodology)  
6. [Usage](#usage)  
7. [Results & Evaluation](#results--evaluation)  
8. [Submission Format](#submission-format)  
9. [Acknowledgments](#acknowledgments)  

---

## 🔍 Overview

This project tackles the Kaggle “House Prices – Advanced Regression Techniques” challenge:

> A playground competition with 79 explanatory variables describing almost every aspect of residential homes in Ames, Iowa. The goal is to predict each home’s final sale price.  

This project is designed to learn:

- Performing **creative feature engineering**  
- Training and tuning **advanced regression models** (Random Forest, XGBoost, Gradient Boosting)  
- Evaluating on **Root-Mean-Squared-Error (RMSE)** of log-prices  

---

## 🗂 Project Structure
- ├── data_description.txt # Data dictionary for all features
- ├── train.csv # Training set (with SalePrice)
- ├── test.csv # Test set (without SalePrice)
- ├── sample_submission.csv # Example submission format
- ├── output.csv # Final model predictions
- └── Advanced_Regression.ipynb # Jupyter notebook walkthrough


---

## 📊 Data
- train.csv – 1,460 samples with SalePrice.
- test.csv – 1,459 samples without SalePrice.
- sample_submission.csv – Id,SalePrice format.
- A complete feature dictionary is provided in data_description.txt.

## 🛠 Methodology
- Exploratory Data Analysis
- Identify missingness, distributions, correlations.
- Visualize with histograms, heatmaps.
- Feature Engineering
- Impute or flag missing values.
- Transform skewed numeric features (e.g., log, Box–Cox).
- Encode categoricals (Ordinal, One-Hot).
- Model Training
- Linear Regression (baseline).
- Random Forest Regressor – tree-based ensemble.
- XGBoost Regressor – gradient boosting with regularization.
- Hyperparameter Tuning
- Grid search / randomized search on key parameters.
- Cross-validation to guard against overfitting.
- Ensembling (optional)
- Blend predictions of multiple models for robustness.

## ▶️ Usage
### Open the Jupyter notebook:
jupyter notebook Advanced_Regression.ipynb

### Run cells in order to:
- Load data (train.csv, test.csv)
- Perform EDA & feature engineering
- Train and evaluate models
- Generate output.csv with final predictions
- Submit output.csv to the Kaggle competition for leaderboard scoring.

## 🏆 Results & Evaluation
- Metric: RMSE of log(predicted) vs. log(actual) sale prices.
- Baseline (Linear Regression): ~0.160 RMSE
- Random Forest: ~0.112 RMSE
- XGBoost: ~0.105 RMSE
- Ensemble: ~0.101 RMSE

## 📂 Submission Format
- csv
- Id,SalePrice
- 1461,169000.1
- 1462,187724.1233
- 1463,175221
…
See output.csv for an example.

## 🙏 Acknowledgments
- Dataset: Ames Housing compiled by Dean De Cock (alternative to Boston Housing).
- Photo: “House in Ames, Iowa” by Tom Thain on Unsplash.
- Tutorials & Inspiration: Kaggle Learn, community kernels on advanced regression techniques.
