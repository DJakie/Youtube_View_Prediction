### YouTube Views Prediction Project

**Objective**: To predict YouTube video views using advanced machine learning techniques and exploratory data analysis (EDA).

**Key Insights from EDA**:
- Metrics like views, likes, and shares exhibit right-skewed distributions.
- Minimal engagement was observed, with over 75% of videos receiving no likes or comments.
- Playlist activity and watch time are dominated by non-premium users.
- Subscriber impact is minimal, with only a few videos significantly affecting subscriber counts.

**Modeling and Results**:
- Tested multiple models, including Linear Regression, Decision Trees, Random Forest, and XGBoost.
- Used 5-fold cross-validation to fine-tune the XGBoost model.
- **XGBoost** achieved the best performance with hyperparameter tuning:
  - **Train R²**: 0.9991 | **Test R²**: 0.9921
  - **Train RMSE**: 0.0862 | **Test RMSE**: 0.2160
  - **MAPE**: ~0.32% on test data


**Feature Importance**:
The most impactful features include:
1. Estimated watch time
2. Videos added to playlists
3. Views from premium users (RedViews)

**Conclusion**:
The XGBoost model demonstrated exceptional accuracy and generalizability, making it a robust solution for predicting YouTube views.


