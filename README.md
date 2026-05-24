# Insurance Charges Prediction Using Machine Learning

## Project Overview

This project focuses on predicting medical insurance charges using Machine Learning techniques. The objective is to analyze how factors such as age, BMI, smoking habits, gender, number of children, and region affect insurance costs.

The project demonstrates a complete end-to-end machine learning workflow including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preprocessing
- Model Building
- Model Evaluation
- Model Comparison

---

# Problem Statement

Medical insurance companies determine insurance charges based on multiple personal and health-related factors. The goal of this project is to build a regression-based machine learning model capable of predicting insurance charges accurately using demographic and health information.

---

# Dataset Information

The dataset contains the following features:

| Feature | Description |
|---|---|
| age | Age of the individual |
| sex | Gender of the individual |
| bmi | Body Mass Index |
| children | Number of children/dependents |
| smoker | Smoking status |
| region | Residential region |
| charges | Medical insurance charges (Target Variable) |

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

# Project Workflow

## 1. Data Understanding
- Loaded and explored the dataset
- Checked dataset shape, columns, and datatypes
- Generated statistical summaries

## 2. Data Cleaning
- Checked missing values
- Removed duplicate records
- Identified numerical and categorical features

## 3. Exploratory Data Analysis (EDA)
Performed:
- Univariate Analysis
- Bivariate Analysis
- Correlation Analysis
- Outlier Detection

Visualizations used:
- Histograms
- Scatterplots
- Boxplots
- Countplots
- Heatmaps

---

# Key Insights from EDA

- Insurance charges tend to increase with age.
- Smokers have significantly higher insurance charges.
- BMI has a moderate positive relationship with insurance charges.
- Obese individuals generally exhibit higher medical costs.
- Region and gender show relatively lower impact on charges.

---

# Feature Engineering

Additional features were created to improve business understanding and model performance.

### BMI Category
BMI values were categorized into:
- Underweight
- Normal
- Overweight
- Obese

### Family Size
A new feature called `family_size` was created using:

```python
family_size = children + 1
```

---

# Data Preprocessing

The following preprocessing steps were applied:

- Label Encoding
- One-Hot Encoding
- Train-Test Split
- Feature Scaling using StandardScaler

---

# Machine Learning Models Used

The following regression models were trained and evaluated:

| Model |
|---|
| Linear Regression |
| Polynomial Regression |
| Random Forest Regressor |

---

# Evaluation Metrics

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

# Model Performance Summary

| Model | Performance |
|---|---|
| Linear Regression | Baseline model |
| Polynomial Regression | Improved non-linear learning |
| Random Forest Regressor | Best overall performance |

---

# Final Conclusion

This project successfully demonstrated the complete machine learning pipeline for predicting insurance charges.

Major findings include:

- Smoking status is the strongest factor affecting insurance charges.
- Feature engineering improved interpretability and analysis.
- Ensemble learning methods like Random Forest significantly improved predictive accuracy.
- Polynomial Regression captured non-linear relationships better than standard Linear Regression.

The project highlights practical applications of:
- Data Analysis
- Machine Learning
- Feature Engineering
- Regression Modeling

---

# Future Improvements

Possible future enhancements include:

- Hyperparameter Tuning
- Cross Validation
- Model Deployment using Streamlit
- Advanced Ensemble Models
- Dashboard Integration using Power BI or Tableau

---

# How to Run the Project

## Clone the Repository

```bash
git clone https://github.com/your-username/Insurance-Charges-Prediction.git
```

## Install Required Libraries

```bash
pip install -r requirements.txt
```

## Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
insurance_charges_prediction.ipynb
```

---

# Project Structure

```text
Insurance-Charges-Prediction/
│
├── insurance_charges_prediction.ipynb
├── insurance.csv
├── insurance_model.pkl
├── README.md
└── requirements.txt
```

---


