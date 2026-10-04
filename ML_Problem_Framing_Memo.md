# ML Problem-Framing Memo

## Problem

The goal is to identify customers who may be at risk of
churning so that the company can provide appropriate
retention support.

## Decision

The business wants to decide which customers should be
considered for proactive retention support.

## Prediction Target

The target variable is `churned`.

- 1 = customer churned
- 0 = customer did not churn

## Unit of Observation

One row represents one customer.

## Features

The features are:

- tenure_months
- support_tickets
- monthly_spend_inr
- last_login_days
- plan_type

`customer_id` is excluded because it is only an identifier.

## Action Window

The prediction should be made before the customer churns,
so that the company has an opportunity to provide retention
support.

## Non-ML Baseline

A simple rule-based baseline is:

If `last_login_days > 14` and `support_tickets >= 3`,
the customer is flagged as high risk.

## False Positive Cost

A false positive may cause unnecessary retention outreach
or incentives.

For this demonstration, the estimated cost is ₹100.

## False Negative Cost

A false negative means a customer at risk of churn is missed.

For this demonstration, the estimated cost is ₹500.

## ML Justification

The current dataset contains only 12 customers.

Therefore, machine learning is not justified for production
deployment using this dataset.

A larger and more representative historical dataset should
be collected before production ML is considered.

The current dataset can be used to demonstrate the ML
problem-framing and responsible-data workflow.
