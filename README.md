# Airbnb-Price-Prediction-and-Insights
A machine learning project to predict Airbnb listing prices using data preprocessing, feature engineering, and a Random Forest model. Achieves strong predictive performance with an R² score of 0.72.

# 🏡 Airbnb Price Prediction

This project focuses on building a regression model to accurately predict the price of Airbnb listings based on various property, host, and location-based features. It was developed as part of an academic assignment aimed at applying machine learning techniques for real-world applications in the travel and rental industry.

---

## 🎯 Problem Statement

The primary objective of this project is to develop a predictive model that estimates the price of an Airbnb listing using a wide range of features including:

- Property type
- Room type
- Number of reviews
- Location (latitude, longitude)
- Amenities and host details

The insights from this analysis are intended to help Airbnb hosts make informed, data-driven decisions regarding pricing, and also to improve Airbnb’s own recommendation systems to enhance host and guest satisfaction.

---

## 📦 Dataset Information

- **Dataset Name**: `airbnb_data.csv`
- **Total Entries**: 74,111
- **Features**: 29  
  The dataset includes property attributes, geographic information, host activity, and user reviews.

---

## 📈 Project Deliverables

1. **Data Exploration and Preprocessing**
   - Identified trends, missing values, and outliers
   - Cleaned the dataset and filled missing numerical values using mean imputation
   - Encoded categorical variables using `LabelEncoder`
   - Engineered new features such as:
     - `num_amenities`: number of amenities per listing
     - `host_activity`: days since last review
   - Applied one-hot encoding to extract individual amenities
   - Normalized features using `StandardScaler`

2. **Model Development**
   - **Model Used**: `RandomForestRegressor` from `scikit-learn`
   - **Data Split**:
     - 70% Training
     - 15% Validation
     - 15% Testing
   - Converted `log_price` into the target variable for better regression handling

3. **Model Evaluation**
   - Performance evaluated using:
     - **RMSE (Root Mean Squared Error)**: 0.38
     - **MAE (Mean Absolute Error)**: 0.28
     - **R² Score**: 0.72
   - Visualizations:
     - Actual vs Predicted Scatter Plot
     - Residual Histogram
     - Feature Importance Bar Chart



---

## ✅ Success Criteria

- Achieved strong performance on test data (R² ≥ 0.70)
- Delivered interpretable insights on what factors most influence Airbnb prices
- Model provides reliable predictions for new or unseen listings

---

## 🔍 Key Insights

- **Top 5 Most Important Features**:
  1. Room type
  2. Bathrooms
  3. Longitude
  4. Latitude
  5. Accommodates

These features were found to have the highest influence on predicting prices, indicating that both property characteristics and geographic location play a crucial role.

---

## ⚙️ Tools and Libraries Used

- **Programming Language**: Python
- **Libraries**:
  - `pandas`, `numpy` – data manipulation
  - `scikit-learn` – modeling and evaluation
  - `matplotlib`, `seaborn` – visualizations

---



