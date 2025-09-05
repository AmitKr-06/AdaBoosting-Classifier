# AdaBoosting-Classifier

Breast Cancer Classification (AdaBoost)

 ## Overview

This project focuses on classifying breast tumors as Malignant (0) or Benign (1) using the Breast Cancer Dataset.
After performing EDA and preprocessing, I trained an AdaBoost Classifier, which achieved 97% accuracy.

## Dataset

Source: scikit-learn’s built-in Breast Cancer Dataset

Features: 30 numeric features

Examples: mean radius, mean texture, mean area, worst concave points

## Target:

0 → Malignant

1 → Benign

Samples: 569 rows × 30 features

##  Exploratory Data Analysis (EDA)

-> Univariate Analysis → Histograms & KDE plots of key features

-> Bivariate Analysis → Pairplots of top features (e.g., mean radius, mean area)

-> Multivariate Analysis → Correlation heatmap

-> PCA → Reduced features for visualization (2D scatter plot)

##  Preprocessing

-> Checked for missing values → none found 

-> Standardized numerical features using StandardScaler

-> Train-test split (80/20)

## Model Training

-> Algorithm: AdaBoostClassifier (base estimator = Decision Tree)

-> Parameters: default (can be tuned with n_estimators, learning_rate)

## Results

-> Accuracy: 97.4%

-> Confusion Matrix:

[[41  2]
 [ 1 70]]


## Classification Report:

-> Precision (Malignant): 0.98 | Recall: 0.95 | F1-score: 0.96

-> Precision (Benign): 0.97 | Recall: 0.99 | F1-score: 0.98

## Visualizations

-> Pairplot of selected important features

-> Correlation heatmap

-> PCA visualization (2D scatter plot)

## Confusion matrix heatmap

## Key Insights

-> AdaBoost achieved 97% accuracy with minimal errors

-> PCA clearly separated the two classes in reduced dimensions

-> Strong potential for use in medical diagnosis applications
