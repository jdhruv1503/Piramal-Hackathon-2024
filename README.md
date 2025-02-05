# Credit Default Probability Prediction System
Piramal Finance Hackathon 2024 - Finalist Submission

## Overview
This project implements a machine learning pipeline to predict credit default probabilities. The system processes financial data through multiple stages of preprocessing, feature engineering, and model training to generate accurate default risk predictions.

## Pipeline Structure

The ML pipeline consists of the following key components:

1. **Exploratory Data Analysis** (`EDA.ipynb`)
   - Initial data exploration and statistical analysis
   - Distribution analysis of key features
   - Correlation studies
   - Missing value analysis

2. **Data Preprocessing** (`Preprocessing.ipynb`)
   - Data cleaning and standardization
   - Handling missing values (initial pass)
   - Format standardization
   - Data validation checks

3. **Advanced Imputation** (`Imputation.ipynb`, `Impute2.ipynb`)
   - Multi-stage imputation strategy
   - Statistical imputation methods
   - Domain-specific imputation rules
   - Data quality validation

4. **Feature Engineering** (`Aggregation, Impute2, Scaling.ipynb`)
   - Feature aggregation and grouping
   - Feature scaling and normalization
   - Feature selection
   - Dimensionality handling

5. **Model Training** (`Model Training.ipynb`)
   - Model selection and hyperparameter tuning
   - Cross-validation implementation
   - Performance metrics evaluation
   - Model validation

6. **Inference Pipeline** (`Inference.ipynb`)
   - Production-ready inference code
   - Model loading and prediction
   - Output formatting
   - Batch prediction capabilities

## Technical Details

### Data Processing Techniques
- Missing value imputation using statistical methods
- Feature scaling using StandardScaler/MinMaxScaler
- Categorical encoding techniques
- Outlier detection and handling

### Feature Engineering Approach
- Temporal feature creation
- Statistical aggregations
- Domain-specific feature construction
- Feature importance analysis

### Model Architecture
- Primary model: XGBoost+LightGBM+CatBoost ensemble with Logistic Regression as meta model
- Cross-validation strategy: K-fold
- Evaluation metrics:
  - ROC-AUC
  - Precision-Recall
  - F1 Score
  - Custom business metrics
