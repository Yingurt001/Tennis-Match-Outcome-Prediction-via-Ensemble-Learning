# Tennis Match Outcome Prediction via Ensemble Learning

## 📌 Overview
This project develops a predictive model for professional tennis match outcomes by integrating multiple ensemble learning methods. Using historical ATP and WTA match data, we extract player-specific and match-specific features, optimize model performance through hyperparameter tuning, and evaluate predictive accuracy across different tournament surfaces.  
> Independent research project (2024) focused on data-driven sports analytics.

## 📂 Contents
- **Data collection**: Historical match statistics from ATP/WTA sources.
- **Feature engineering**: Player performance metrics, surface-adjusted stats, fatigue index.
- **Modeling**: Gradient Boosting, Random Forest, Logistic Regression.
- **Model evaluation**: Nested cross-validation, accuracy and ROC-AUC.
- **Interpretability**: Feature importance analysis for performance drivers.

## 📊 Methodology
1. **Data Acquisition & Cleaning**
   - Collected match results, player rankings, and in-match statistics (serve %, aces, break points).
   - Removed incomplete records and standardized feature formats.

2. **Feature Engineering**
   - Constructed **serve performance metrics** (first serve %, ace rate, double fault rate).
   - Built **return performance indicators** (break point conversion, return points won).
   - Added **fatigue index** based on consecutive matches, travel distance, and tournament stage.
   - Adjusted player stats for **court surface** (hard, clay, grass).

3. **Modeling Approach**
   - Implemented three base models:
     - **Gradient Boosting Classifier** (XGBoost/LightGBM)
     - **Random Forest Classifier**
     - **Logistic Regression**
   - Combined predictions using **soft voting** ensemble method.

4. **Hyperparameter Tuning & Validation**
   - Applied nested cross-validation (outer loop for evaluation, inner loop for tuning).
   - Optimized parameters such as learning rate, max depth, and regularization strength.

5. **Model Interpretation**
   - Used permutation feature importance and SHAP values to identify key factors influencing match outcome predictions.
   - Found serve-related metrics and surface-adjusted performance indicators as top predictors.

## 📈 Key Results
- **Best Accuracy**: 85% on Grand Slam test set.
- **Top Features**:
  - First serve win percentage
  - Break point conversion rate
  - Surface-adjusted win rate
  - Fatigue index
- Performance varies by surface, with higher predictive accuracy on hard and grass courts than clay.

## 🛠️ Reproducibility
**Requirements**
```bash
python>=3.10
pandas
numpy
scikit-learn
xgboost
lightgbm
matplotlib
seaborn
shap
