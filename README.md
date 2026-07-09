# Claim Severity Modeling

## Project Overview

This project compares three statistical models for predicting insurance claim severity using the AutoClaims dataset in R.

The objective is to evaluate the strengths and limitations of:

- Ordinary Least Squares (OLS)
- Log-transformed Linear Regression
- Gamma Generalized Linear Model (Gamma GLM)

and determine which model is most appropriate for claim severity modeling.

---

## Dataset

- **Dataset:** AutoClaims (insuranceData package)
- **Response Variable:** PAID (Claim Severity)
- **Predictors:** State, Class, Gender, and Age

---

## Methodology

The following models were developed and compared:

1. Linear Regression (OLS)
2. Log-transformed Linear Regression
3. Gamma GLM with a Log Link

The comparison focuses on:

- Distributional assumptions
- Prediction behavior
- Heteroskedasticity
- Retransformation bias
- Suitability for insurance claim severity modeling

---

## Key Findings

- OLS provides a useful baseline model but is not well suited for highly skewed insurance claim data.
- Log transformation reduces skewness and improves model assumptions but introduces retransformation bias.
- Gamma GLM models claim severity directly on the original scale while naturally handling positive, right-skewed claim amounts.

---

## Files

- `Claim_Severity_Modeling.Rmd` — R Markdown source
- `Claim_Severity_Modeling.html` — Full project report
- `style.css` — Custom report styling

---

## Software

- R
- R Markdown
- insuranceData
- car
- moments
