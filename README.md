# MIS_Assignment

## Problem Statement
The goal is to classify 2,627 potential customers in a new market into four predefined segments (A, B, C, D). The segmentation strategy is based on a dataset of 8,068 individuals from the current market.


## Steps Followed

1. **Data Preprocessing**:
    - Imputed missing values for numerical features using the median.
    - Imputed missing values for categorical features using the mode.
    - Encoded categorical variables using appropriate techniques (e.g., label encoding, one-hot encoding).
    - Scaled numerical features using `MinMaxScaler`.

2. **Exploratory Data Analysis (EDA)**:
    - Examined the distribution of features using count plots and summary statistics.
    - Visualized correlations and missing values using heatmaps.

3. **Model Development**:
    - Experimented with multiple classifiers: Random Forest, Gradient Boosting, SVM, Logistic Regression, KNN, XGBoost, and LightGBM.
    - Identified **Gradient Boosting** as the best model with an accuracy of **53%**.
    - Applied dimensionality reduction techniques (PCA) and clustering algorithms (k-means, DBSCAN) for additional insights.
    - Performed hyperparameter tuning using grid search.

4. **Test Set Predictions**:
    - Preprocessed the test dataset with the same pipeline as training data.
    - Generated predictions using the Gradient Boosting model.
    - Mapped numeric labels back to categorical values (A/B/C/D).
    - Saved results to `test2_predictions.csv`.
