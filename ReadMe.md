# Space Ship Titanic — Machine Learning Project

This repository contains a complete end-to-end data science workflow for the **Space Ship Titanic** dataset. The project focuses on data cleaning, exploratory data analysis (EDA), feature engineering, and machine learning model experimentation for a supervised classification task.





---

## Repository Structure

```
space_ship_titanic/
├── cleaned_data/                         # Cleaned and processed datasets
├── data_source__spaceship-titanic/       # Raw source data files
├── model_experiments/                    # Trained models and experiment artifacts
├── Data_cleaning_and_EDA.ipynb           # Main analysis and EDA notebook
├── requirements.txt                     # Python dependencies
└── README.md                             # Project documentation
```

---

## Project Overview

The objective of this project is to predict passenger outcomes using the Space Ship Titanic dataset. The dataset contains a mixture of numerical and categorical features, requiring careful preprocessing and feature engineering before model training.

The project emphasizes:

- Reproducible data preprocessing pipelines
- Clear exploratory data analysis
- Robust feature engineering
- Comparison of multiple machine learning models

---

## Data Description

### Data Source --> Kaggle: https\://www\.kaggle.com/competitions/spaceship-titanic/data

Contains the original dataset files used as input to the project. These files are not modified directly and serve as the raw data source for all downstream processing.

### `cleaned_data/`

Contains cleaned and transformed versions of the dataset after:

- Handling missing values
- Encoding categorical variables
- Scaling numerical features
- Feature extraction and transformation

These datasets are used directly for modeling.

---

## Analysis Notebook

### `Data_cleaning_and_EDA.ipynb`

This notebook documents the full analytical workflow, including:

1. **Data Loading**

   - Reading raw CSV files
   - Initial inspection of schema and data types

2. **Data Cleaning**

   - Missing value imputation
   - Feature normalization and scaling
   - Categorical encoding using `ColumnTransformer`

3. **Exploratory Data Analysis (EDA)**

   - Feature distributions
   - Target variable balance
   - Correlation analysis
   - Visualizations using matplotlib and seaborn

4. **Feature Engineering**

   - Derived variables
   - Cabin feature decomposition
   - Pipeline-based preprocessing

---

## Model Experiments

### `model_experiments/`

This directory contains saved models and experiment outputs generated during training and evaluation. Models are trained using scikit-learn pipelines and include both baseline and advanced approaches.

Models and artifacts are typically serialized using `joblib` for reuse and evaluation.

---

## Dependencies

The project uses the following Python libraries:

```
pandas==2.3.3
numpy==2.4.0
matplotlib==3.10.8
seaborn==0.13.2
scikit-learn==1.8.0
xgboost==3.1.2
joblib==1.5.3
```

All dependencies are listed in `requirements.txt`.

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/rick-a-commits/space_ship_titanic.git
cd space_ship_titanic
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open and run the notebook:

```bash
jupyter notebook Data_cleaning_and_EDA.ipynb
```

---

## Notes and Future Work

Potential next steps include:

- Model explainability (e.g., SHAP)
- Exporting predictions for downstream use

---

##

