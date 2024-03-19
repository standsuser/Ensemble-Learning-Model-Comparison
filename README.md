# Ensemble Learning Model Comparison

This repository contains code for comparing the performance of ensemble learning models on three different datasets: Banknote Authentication, Bankloan, and Glasstype Prediction. Ensemble learning models, including Random Forest, AdaBoost, and Gradient Boosting, are implemented and evaluated on each dataset.

## Datasets

- **Banknote Authentication Dataset**: This dataset contains features extracted from photographic images of genuine and forged banknotes. The task is to predict whether a banknote is authentic or forged based on these features.

- **Bankloan Dataset**: This dataset contains information about customers' demographics, financial status, and other factors, with the target variable indicating whether the customer accepted a personal loan offer.

- **Glasstype Prediction Dataset**: This dataset includes various attributes related to glass manufacturing processes, with the goal of predicting the type of glass based on these attributes.

## Preprocessing Steps

### Banknote Authentication Dataset
- Checked for missing values.
- Visualized and removed outliers using the Interquartile Range (IQR) method.
- Normalized the numerical features using z-score.
- Applied Ridge regularization to handle potential multicollinearity.

### Bankloan Dataset
- Handled missing values.
- Dropped unnecessary columns.
- Scaled numerical features using StandardScaler.
- Utilized Elastic Net regularization to address potential collinearity.

### Glasstype Prediction Dataset
- Detected and removed outliers using the IQR method.
- Applied Ridge regularization to handle potential collinearity.

## Hyperparameter Tuning Process

For each dataset and ensemble model, a GridSearchCV approach was employed to tune hyperparameters and find the optimal settings. The following hyperparameters were tuned for each model:

- **Random Forest**: Number of estimators, maximum depth, minimum samples split, and minimum samples leaf.
- **AdaBoost**: Number of estimators and learning rate.
- **Gradient Boosting**: Number of estimators, learning rate, maximum depth, and minimum samples split.

## Results

The accuracy, precision, recall, and F1-score metrics were calculated for each ensemble model on each dataset. The results are summarized in tables and visualized using bar charts and heatmaps.

## Insights

The comparison of ensemble learning models across different datasets provides insights into the performance variations based on dataset characteristics and model suitability. These insights can inform the selection of appropriate models for specific predictive tasks and datasets.

## Contributors

- Mariam Sherif Almotawally
- Feras Nezar Elkharrat
- Rita Emad Roshdy


