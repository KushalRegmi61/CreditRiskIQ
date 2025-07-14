# Credit Card Fraud Detection Project

This project implements a machine learning pipeline for credit card fraud detection using various features like debt ratio, income, age, and payment history.

## Project Structure

```
│
├── data/
│   └── loan_data.csv                 # 10K sampled dataset
├── notebooks/
│   └── 01_eda_and_preprocessing.ipynb
│   └── 02_pipeline_training.ipynb
├── src/
│   ├── preprocess.py                 # Custom transformers
│   ├── pipeline.py                   # Pipeline creation
├── outputs/
│   └── model.pkl                     # Final saved model
│
├── requirements.txt
├── README.md
```

## Dataset Features

- **SeriousDlqin2yrs**: Target variable (1 = serious delinquency, 0 = no delinquency)
- **RevolvingUtilizationOfUnsecuredLines**: Credit utilization ratio
- **age**: Age of the borrower
- **NumberOfTime30-59DaysPastDueNotWorse**: Number of times 30-59 days past due
- **DebtRatio**: Total debt to income ratio
- **MonthlyIncome**: Monthly income
- **NumberOfOpenCreditLinesAndLoans**: Number of open credit lines
- **NumberOfTimes90DaysLate**: Number of times 90+ days late
- **NumberRealEstateLoansOrLines**: Number of real estate loans
- **NumberOfTime60-89DaysPastDueNotWorse**: Number of times 60-89 days past due
- **NumberOfDependents**: Number of dependents

## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run the notebooks in order:
   - `01_eda_and_preprocessing.ipynb` for data exploration
   - `02_pipeline_training.ipynb` for model training

## Model Pipeline

The pipeline includes:
- Data preprocessing and feature engineering
- Handling missing values
- Feature scaling
- Model training with multiple algorithms
- Model evaluation and selection