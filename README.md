# Python_project-ML-

# Predicting Hospital Length of Stay (LOS)

This project aims to predict the hospital Length of Stay (LOS) across various categories using machine learning algorithms. The primary goal is to enhance patient care, improve operational efficiency, and optimize resource allocation in hospitals.

## Abstract

The hospital Length of Stay (LOS) across categories such as short, medium, long, very long, and prolonged stays can be predicted using machine learning algorithms described in this project. The project enhances patient care, operational efficiency, and resource allocation in hospitals while addressing significant challenges in healthcare administration.

Hospital data from New York State (2015) was carefully examined, followed by data preparation and the application of Synthetic Minority Over-sampling Technique (SMOTE) to balance the dataset. Three machine learning models—Ordinal Logistic Regression, Decision Tree Classifier, and XGBoost—were used and evaluated. The XGBoost model, particularly after hyperparameter tuning, performed most effectively in accurately predicting LOS in various categories.

## Methodology

### Data Description

The project used detailed information on hospital patient discharges from New York State in 2015. Obtained from the Statewide Planning and Research Cooperative System (SPARCS), this dataset contains 1,045,306 records and 34 variables, including treatment details and clinical specialties.

### Data Cleaning Process

Data cleaning ensures data quality by properly coding and maintaining consistency, handling missing data, and removing redundancy to improve model performance and sample size. This initial stage impacts the integrity and reliability of all subsequent explorations.

### Feature Engineering

The 'Length of Stay' field was transformed to classify it properly within the dataset. Entries like '120+' were encoded numerically to 120. Categories in the 'Stay Category' column were ordinally encoded to reflect their natural order (e.g., 'Short stay' encoded as 0, 'Medium stay' as 1).

### Exploratory Data Analysis

EDA provided an in-depth analysis of the variables, their categories, and classification, laying the foundation for subsequent research steps. Statistical analysis was performed on numeric data.

### Model Training and Evaluation

1. **Initial Model Trials with Unbalanced Data**: Various prediction models were applied to the unbalanced dataset to create an initial benchmark.
2. **Feature Selection with SMOTE (Balanced Data)**: Balanced data was used to perform feature selection, reducing overfitting and improving precision. SMOTE ensured key factors were employed in model training.
3. **Hyperparameter Tuning of the Best-Performing Model**: The best-performing model from the initial trials underwent hyperparameter tuning to optimize predictive performance.

## Results

The following are the key results from the models used in this project:


These results indicate that the XGBoost model is the most suitable for this prediction task, providing accurate predictions and helping to improve patient care planning and hospital resource management.


