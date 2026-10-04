# Customer Churn ML — Responsible Problem Framing

## Project Overview

This project demonstrates responsible machine learning
problem framing for customer churn prediction.

The goal is to determine whether machine learning is
justified before deploying a model.

## Dataset

The dataset contains 12 customer records with:

- Customer tenure
- Support tickets
- Monthly spending
- Last login activity
- Plan type
- Churn status

## Project Files

- `baseline_customer_churn.ipynb` — baseline analysis and evaluation
- `ML_Problem_Framing_Memo.md` — problem framing
- `Responsible_Data_Card.md` — responsible data documentation
- `Risk_Register.md` — risks and safeguards

## Baseline

A simple rule-based baseline flags a customer as high risk
when:

`last_login_days > 14` AND `support_tickets >= 3`

## Important Limitation

The dataset contains only 12 customers.

Therefore, it is suitable for demonstrating the workflow,
but it is not sufficient for reliable production ML.

A larger and more representative dataset would be required
before deployment.

## Responsible ML

The project considers:

- False positives
- False negatives
- Data leakage
- Privacy
- Bias
- Human review
- Monitoring
- Rollback conditions
