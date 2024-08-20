# ETL-Pipeline
Build an ETL Pipeline that loads, preprocesses, and enhances data with this pipeline. It supports CSV, Excel, and JSON formats, handles missing values, scales features, encodes categories, adds polynomial features, and applies PCA. Validates data at each step and saves results. Suitable for smaller datasets

## Features

- **Data Loading**: 
  - Supports multiple file formats including CSV, Excel (`.xls` and `.xlsx`), and JSON.

- **Preprocessing**:
  - Handles missing values by imputing with the mean of numerical columns.
  - Standardizes numerical features using z-score normalization.
  - Encodes categorical variables using one-hot encoding.

- **Feature Engineering**:
  - Adds polynomial features to capture non-linear relationships.
  - Applies Principal Component Analysis (PCA) for dimensionality reduction, useful for visualization and reducing feature space.

- **Validation**:
  - Validates data at various stages to ensure correctness:
    - Checks missing values post-imputation.
    - Prints shapes and feature counts after transformations.
    - Outputs explained variance from PCA.

- **Data Saving**:
  - Saves the processed data back to CSV, Excel, or JSON formats.
