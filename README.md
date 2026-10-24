# Machine Learning Model Comparison

## Overview
This project compares baseline and machine learning models across four datasets, covering classification, regression, and time-series forecasting.

## Datasets
- **Adult Income:** Classification
- **Breast Cancer Wisconsin:** Classification
- **Red Wine Quality:** Regression
- **Daily Minimum Temperatures:** Time-series forecasting

## Models

### Classification
- Majority Class Baseline
- Logistic Regression
- Decision Tree Classifier

### Regression
- Mean Baseline
- Ridge Regression
- Decision Tree Regressor

## Evaluation Metrics

**Classification:** Accuracy, Precision, Recall, F1-score, ROC-AUC, and Matthews Correlation Coefficient (MCC).

**Regression:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R², and Mean Absolute Percentage Error (MAPE).

## Validation
Classification experiments use stratified cross-validation. The temperature forecasting experiment uses chronological time-series cross-validation to avoid training on future observations.

An ablation study evaluates Ridge Regression using one, two, and three previous-day temperature features.

## Repository Structure
- `notebooks/` — experiment notebooks
- `results/` — CSV files containing experimental results
- `figures/` — visualizations
- `paper/` — research paper drafts
- `requirements.txt` — Python dependencies

## Reproducibility
Experiments use fixed random seeds where applicable. Software dependencies are listed in `requirements.txt`.

## Limitations
Results depend on data preprocessing, model configuration, and validation strategy. Further experiments and appropriate statistical analyses are needed before drawing strong conclusions.

## Project Status
Research project in progress. Results are experimental and should not be interpreted as universal claims about model performance.
