# Smart-water-monitoring-system-ML
Water Consumption Prediction Project
====================================

Approach:
---------
1. Data Preprocessing:
   - Handled missing values with KNN imputation for numerical features
   - Used label encoding for categorical variables
   - Applied standardization to all features

2. Feature Engineering:
   - Created interaction features (Residents × Temperature)
   - Added temporal features from timestamps
   - Implemented target encoding for high-cardinality categories

3. Modeling:
   - Random Forest Regressor with 500 trees
   - Time-series cross-validation (5 splits)
   - Hyperparameter tuning using GridSearchCV

Tools Used:
----------
- Python 3.8+
- Scikit-learn 1.0.2
- Pandas 1.4.0
- XGBoost 1.6.0
- Matplotlib 3.5.0

Results:
-------
- RMSE: 11.68
- MAE: 8.42
- R²: 0.91

Usage:
------
1. Install requirements: pip install -r requirements.txt
2. Run pipeline: python predict.py --input test_data.csv
