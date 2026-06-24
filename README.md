# Logistics Analytics & Delay Prediction System

## Project Overview

This project analyzes 99,441 e-commerce orders from the Brazilian Olist dataset to identify logistics bottlenecks, customer satisfaction drivers, revenue concentration risks, and delivery delay patterns.

The project combines:

- Data Cleaning
- Feature Engineering
- PostgreSQL Data Warehouse
- SQL Analytics
- Exploratory Data Analysis (EDA)
- Business Recommendations
- Machine Learning

---

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- PostgreSQL
- SQLAlchemy
- Scikit-Learn
- Jupyter Notebook

---

## Dataset

Source: Olist Brazilian E-commerce Dataset

Dataset Size:

- 99,441 Orders
- 2016–2018
- Multiple Brazilian States

Key Features:

- customer_state
- order_value
- payment_value
- freight_value
- delivery_days
- delay_days
- review_score
- is_late

---

## Project Workflow

1. Data Understanding
2. Data Cleaning
3. Feature Engineering
4. PostgreSQL Warehouse Creation
5. SQL Analytics
6. Visual EDA
7. Business Recommendations
8. Delay Prediction Model

---

## Key Business Insights

### Revenue Concentration

Top 3 states contribute:

62.53% of total revenue

States:

- São Paulo (SP)
- Rio de Janeiro (RJ)
- Minas Gerais (MG)

---

### Customer Satisfaction

Average Review Score:

| Delivery Speed | Review Score |
|---------------|-------------|
| Fast | 4.42 |
| Normal | 4.34 |
| Slow | 4.18 |
| Very Slow | 3.10 |

Finding:

Customer satisfaction decreases significantly as delivery times increase.

---

### Operational Risk States

Highest Late Delivery Rates:

| State | Late Delivery % |
|--------|----------------|
| AL | 20.58 |
| MA | 16.73 |
| SE | 14.57 |
| PI | 13.33 |
| CE | 13.17 |

---

### Revenue Per Order

Highest Revenue Per Order:

- PB
- AC
- AP
- AL
- RO

These regions represent potential premium market opportunities.

---

## Machine Learning

### Problem

Predict whether an order will be delivered late.

Target Variable:

is_late

### Models Used

- Logistic Regression
- Random Forest

---

### Baseline Logistic Regression

| Metric | Value |
|---------|--------|
| Accuracy | 93.37% |
| ROC-AUC | 0.56 |

Observation:

The model struggled due to severe class imbalance.

---

### Improved Random Forest

| Metric | Value |
|---------|--------|
| Accuracy | 90.75% |
| Precision | 19.53% |
| Recall | 12.70% |
| ROC-AUC | 0.687 |

Feature engineering significantly improved model performance.

---

## Top Predictive Features

1. order_value
2. payment_value
3. freight_value
4. purchase_month
5. customer_state

---

## Repository Structure

```text
data/
notebooks/
screenshots/
sql/
README.md
requirements.txt
```

---

## Future Improvements

- Advanced Feature Engineering
- XGBoost Model
- SMOTE Class Balancing
- Automated Data Pipeline

---

## Author

Rishi Verma

Data Analytics | Machine Learning | SQL | Python
