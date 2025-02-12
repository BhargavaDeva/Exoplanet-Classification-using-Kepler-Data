# Exoplanet-Classification-using-Kepler-Data
Machine learning project for classifying exoplanets using time-series data from the Kepler space telescope


# Exoplanet Classification using Kepler Data

This project uses time-series flux data from the Kepler space telescope to classify stars as having exoplanets or not.

## Dataset
- `exoTrain.csv`: Training data.
- `exoTest.csv`: Testing data.

## Requirements
- Python 3.x
- Libraries: numpy, pandas, scikit-learn, imblearn, xgboost, matplotlib, seaborn


Key Observations
Imbalanced Data:

The dataset is highly imbalanced, with very few exoplanet samples. SMOTE is used to address this issue.

High Accuracy:

Most models achieve high accuracy (>97%), but this is primarily due to the dominance of the majority class (non-exoplanets).

Challenges with Minority Class:

Despite high overall accuracy, the models struggle to correctly classify exoplanets (minority class), as seen in the confusion matrix and classification report.

Dimensionality Reduction:

PCA is effective in reducing the number of features while retaining most of the variance.

Model Performance:

Naive Bayes and XGBoost perform the best, achieving 99.12% accuracy.
