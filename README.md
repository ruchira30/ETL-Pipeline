# ETL-Pipeline

A Python-based ETL pipeline for loading, preprocessing, transforming, and exporting structured data. The pipeline supports multiple file formats, handles missing values, scales numerical features, encodes categorical variables, performs feature engineering, and applies PCA for dimensionality reduction.

## Features

* **Data Loading**

  * Supports CSV, Excel (`.xls` and `.xlsx`), and JSON formats.
  * Automatically detects the input format from the file extension.

* **Data Preprocessing**

  * Handles missing numerical values using mean imputation.
  * Standardizes numerical features using `StandardScaler`.
  * Encodes categorical variables using one-hot encoding.

* **Feature Engineering**

  * Generates squared polynomial features to expand the feature space.
  * Applies Principal Component Analysis (PCA) to reduce the feature space to two principal components.
  * Reports the explained variance ratio of the PCA components.

* **Validation**

  * Reports the initial dataset shape and column types.
  * Checks for missing values after imputation.
  * Reports the number of features after preprocessing and feature engineering.
  * Outputs the explained variance ratio from PCA.

* **Data Export**

  * Saves the transformed data to CSV, Excel, or JSON.
  * Automatically determines the output format from the file extension.

## Pipeline

**Extract → Transform → Load**

1. Load data from CSV, Excel, or JSON.
2. Preprocess numerical and categorical features.
3. Handle missing values and standardize numerical features.
4. Apply one-hot encoding to categorical features.
5. Generate polynomial features.
6. Apply PCA for dimensionality reduction.
7. Save the transformed dataset in the desired format.

Suitable for **small and structured datasets requiring a reusable preprocessing and feature engineering pipeline**.
