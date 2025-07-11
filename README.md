# 🎧 Podcast Listening Time Prediction - Machine Learning Project

## 🏁 Project Overview

This repository contains my submission for a Kaggle competition focused on **predicting how long users will listen to a podcast episode**. Using a rich dataset with 70+ features and 700K+ records, this machine learning pipeline leverages data preprocessing, feature engineering, and model experimentation to forecast episode listening durations accurately.

## 📦 Dataset

The dataset includes various features related to:
- **User behavior**
- **Device metadata**
- **Episode characteristics**
- **Listening history**

> 🔒 Due to competition rules, the dataset is not publicly available here. Please refer to the official Kaggle competition page for access.

---

## 🚀 Workflow

### 1. **Exploratory Data Analysis (EDA)**
- Handled missing values and data imbalance.
- Studied target variable distribution (`Episode_Length`).
- Correlation matrix for numerical features.
- Visualized distributions and outliers.

### 2. **Preprocessing**
- Dropped unnecessary columns (`Episode_Title` etc.).
- Converted boolean columns to numerical (True → 1, False → 0).
- Label encoded categorical columns.
- Scaled numerical features using `StandardScaler`.

### 3. **Feature Engineering**
- Created new interaction and ratio-based features.
- Extracted day, hour, and weekday patterns.
- Reduced multicollinearity using VIF filtering.

### 4. **Modeling**
Experimented with multiple regression algorithms:
- `RandomForestRegressor`
- `XGBoost`
- `LightGBM`
- `CatBoost`
- `Linear Regression`
- `Gradient Boosting Regressor`

Best performing model: **XGBoost Regressor** with RMSE-based tuning.

### 5. **Hyperparameter Tuning**
- Used `GridSearchCV` & `RandomizedSearchCV`.
- Tuned learning rate, depth, estimators.

### 6. **Evaluation**
- Metric used: **Root Mean Squared Error (RMSE)**
- Compared model performance on validation set.
- Cross-validation to avoid overfitting.

---

## 🧠 Technologies Used

| Category       | Libraries & Tools                             |
|----------------|-----------------------------------------------|
| Language       | Python                                        |
| Data Handling  | pandas, numpy                                 |
| Visualization  | matplotlib, seaborn, plotly                   |
| Modeling       | scikit-learn, xgboost, lightgbm, catboost     |
| Preprocessing  | LabelEncoder, StandardScaler                  |

---

## 📈 Results & Insights

- Best RMSE achieved: `XX.XXX` (fill in your score).
- Feature importance showed episode duration, session start time, and user history played key roles.
- Scaling and encoding greatly impacted performance.

---

## 📝 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/sahil007707/podcast-listening-time-ml.git
