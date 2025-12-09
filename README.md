ACIS Insurance Risk Analytics
Project Overview

The goal of this project is to analyze ACIS insurance data to uncover patterns related to risk and profitability. The insights from this analysis aim to support better decision-making for premium adjustments and marketing strategies. This repository contains data, exploratory data analysis (EDA), hypothesis testing, and predictive modeling workflows.

Project Structure
acis-insurance-risk-analytics/
├── data/                        # Raw and processed datasets
│   ├── processed_cleaned_data.csv.dvc
│   └── MachineLearningRating_v3.txt
├── notebooks/                    # Jupyter notebooks for analysis
│   └── task_2_eda.ipynb
├── src/                          # Python modules (planned)
├── .dvc/                         # DVC folder for data versioning
├── .gitignore
├── requirements.txt              # Python dependencies
└── README.md

Key Features
Task 1: Git & Project Setup

Initialized Git repository and set up branch structure (task-1, task-2, task-3-4)

Configured .gitignore for project and DVC cache

Setup DVC for dataset versioning

Task 2: Data Processing & EDA

Cleaned and preprocessed ACIS insurance data

Added processed dataset to DVC

Performed descriptive statistics, missing value checks, and visual exploration
<img width="721" height="473" alt="image" src="https://github.com/user-attachments/assets/c003a7db-8639-48e1-91f0-8b77080a1878" />


Notebook includes univariate and bivariate analysis, outlier detection, and correlation analysis

Task 3: Hypothesis Testing

Conducted statistical tests to evaluate key assumptions:

T-test: Premium differs by Gender

ANOVA: Premium differs by Province

Pearson correlation: Significant correlation between TotalPremium and TotalClaims

Task 4: Predictive Modeling

Implemented a pipeline with preprocessing for numeric and categorical features

Used SimpleImputer, StandardScaler, and OneHotEncoder for feature preprocessing

Trained a LinearRegression model to predict TotalPremium

Handled missing values and inconsistent data types in the dataset

Data Versioning & Large File Handling

Large files are tracked using DVC and Git LFS

.dvc/cache and .dvc/tmp are excluded from Git via .gitignore

Example: data/processed_cleaned_data.csv and data/MachineLearningRating_v3.txt are managed with DVC/Git LFS

Setup Instructions

Clone the repository:

git clone https://github.com/life412/acis-insurance-risk-analytics.git
cd acis-insurance-risk-analytics


Install dependencies:

pip install -r requirements.txt


Install Git LFS (if not already installed):

git lfs install


Pull large datasets via DVC:

dvc pull


Open Jupyter Notebook for EDA:

jupyter notebook notebooks/task_2_eda.ipynb

Next Steps

Create reusable Python modules for EDA (src/eda.py) and predictive modeling (src/model.py)

Extend predictive models with additional features and algorithms

Prepare final report summarizing key insights, statistical tests, and model results
