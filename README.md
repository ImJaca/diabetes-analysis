# Diabetes Data Analysis with Apache Spark

## Project Overview

The goal of this project was to analyze a healthcare dataset containing information about people with diabetes and related health indicators. The analysis was carried out using **Apache Spark (PySpark)** in a **Docker** environment.
demographic factors and diabetes status, and compares machine learning
models for binary classification.

## Dataset

The dataset contains **253,680 records and 22 variables**, including:

-   Diabetes status (no diabetes, prediabetes, or diabetes)
-   Blood pressure and cholesterol
-   BMI, smoking, and physical activity
-   General, mental, and physical health indicators
-   Age, education, and income

No missing values were found during the initial data-quality analysis.

## Analysis Workflow

1.  **Data loading and inspection** -- loading the CSV dataset with
    Spark and examining its schema and descriptive statistics.
2.  **Data quality assessment** -- checking the dataset for missing
    values.
3.  **Exploratory data analysis** -- calculating feature correlations
    and examining selected relationships with the target variable.
4.  **MapReduce analysis** -- using RDD `map()` and `reduceByKey()`
    operations to calculate diabetes prevalence across selected binary
    features.
5.  **Data preparation** -- converting the target into a binary variable
    (no diabetes vs. diabetes/prediabetes), selecting features,
    splitting the data into training and test sets (80/20), and applying
    class weights to address class imbalance.
6.  **Model training** -- training and comparing Logistic Regression and
    XGBoost classifiers.
7.  **Model evaluation** -- comparing AUC-ROC, accuracy, F1-score,
    precision, recall, confusion matrices, and ROC curves.

## Model Results

``` text
.
├── .git/
├── data/
├── docker/
├── notebooks/
├── .gitignore
├── analisys.ipynb
├── README.md
└── requirements
```

## Technologies

-   **Docker** -- containerized project environment
-   **Apache Spark / PySpark** -- data processing and machine learning
-   **Python** -- analysis and supporting scripts
-   **Jupyter Notebook** -- interactive analysis
-   **XGBoost** -- gradient-boosted classification
-   **Pandas, Matplotlib, Seaborn, scikit-learn** -- data handling,
    visualization, and evaluation