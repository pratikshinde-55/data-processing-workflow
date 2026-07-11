# Data Processing Workflow

## Overview

**Data Processing Workflow** is a complete data preprocessing and exploratory data analysis (EDA) project that demonstrates how raw data is transformed into a clean and machine-learning-ready format.

The project focuses on handling real-world data challenges such as data cleaning, feature transformation, encoding categorical variables, outlier detection, feature analysis, and preparing data for machine learning models.

---

## Project Workflow

The complete workflow followed in this project:

```
Raw Data
   |
   ↓
Data Understanding
   |
   ↓
Data Cleaning
   |
   ↓
Exploratory Data Analysis (EDA)
   |
   ↓
Feature Engineering
   |
   ↓
Feature Encoding
   |
   ↓
Feature Selection
   |
   ↓
Processed Dataset
   |
   ↓
Machine Learning Ready Data
```

---

## Features Implemented

### 1. Data Loading & Understanding

* Loaded raw dataset using Pandas.
* Checked dataset structure and information.
* Analyzed columns, data types, and missing values.

### 2. Data Cleaning

Performed data preprocessing steps such as:

* Handling missing values
* Removing duplicate records
* Correcting inconsistent data
* Converting data types where required

### 3. Exploratory Data Analysis (EDA)

Performed analysis using:

* Histograms
* Count plots
* Box plots
* Correlation heatmaps

EDA helped to understand:

* Data distribution
* Feature relationships
* Outliers
* Data patterns

---

## Feature Engineering

Created new meaningful features from existing data.

Examples:

* Converting numerical values into categories
* Creating BMI categories
* Transforming features to improve model understanding

---

## Data Encoding

Machine learning models require numerical input, so categorical features were converted into numerical format.

Techniques used:

### Label Encoding

Converted binary categories into numerical values.

Example:

```
Male   → 0
Female → 1
```

### One-Hot Encoding

Converted categorical variables into dummy variables.

Example:

```
Region
 |
 ↓

region_northwest
region_southeast
region_southwest
```

`drop_first=True` was used to remove one dummy column and avoid redundant information.

---

## Feature Analysis

### Correlation Analysis

Pearson correlation was used to understand the relationship between features and the target variable.

Purpose:

* Identify important features
* Understand feature impact
* Support feature selection

---

### Chi-Square Test

Chi-square test was performed for categorical features.

Purpose:

* Check whether categorical variables have a significant relationship with the target.
* Decide whether a feature should be kept or removed.

---

### Multicollinearity Check

VIF (Variance Inflation Factor) analysis was used to identify highly correlated input features.

Purpose:

* Reduce redundant features
* Improve regression model stability

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy

### Tools

* Jupyter Notebook
* VS Code
* Git & GitHub

---

## Project Structure

```
data-processing-workflow/

│
├── data/
│   ├── raw/
│   │    ├── heart.csv
│   │    └── insurance.csv
│   │
│   └── processed/
│           ├── heart_processed.csv
│           └── insurance-processed.csv
│
├── notebooks/
│   ├── Heart.ipynb
│   └── insurance.ipynb
│
├── requirements.txt
│
└── README.md
```



## Installation & Setup

Clone the repository:

```bash
git clone https://github.com/pratikshinde-55/data-processing-workflow.git
```

Navigate to the project directory:

```bash
cd data-processing-workflow
```

Install required libraries:

```bash
pip install -r requirements.txt
```

Run the Jupyter Notebook:

```bash
jupyter notebook
```

---

## Key Learnings

Through this project, I learned:

* How to clean and preprocess real-world datasets
* How to perform detailed EDA
* How to handle categorical variables
* How to create meaningful features
* How to analyze feature importance
* How to prepare datasets for machine learning models

---

## Future Improvements

* Add automated preprocessing pipeline
* Add machine learning model training
* Add model evaluation metrics
* Deploy preprocessing workflow using Flask/FastAPI
* Implement ML pipeline using Scikit-learn Pipeline

---

## Author
**Pratik Shinde**


