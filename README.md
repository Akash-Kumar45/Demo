# LifeShield Mortality Risk Predictor

## Overview
LifeShield Mortality Risk Predictor estimates 1-year mortality risk for life insurance underwriting.

## Business Objective
Support underwriters with a risk score and risk band (Low/Medium/High) to improve consistency and turnaround time.

## Human Oversight
This model is decision-support only. Final underwriting approval remains with a human underwriter.

## Inputs
- Age
- Gender
- Smoking status
- BMI
- Diabetes / Hypertension / Cardiac history flags
- Lab summary score
- Policy attributes (sum assured, term, product type)

## Outputs
- Mortality risk score (0-1)
- Risk band: Low / Medium / High

## Data Sources
- Historical policy applications (2018-2024)
- Claims outcomes
- Underwriting decision history

## Monitoring
- Monthly drift checks
- Quarterly calibration checks
- Fairness checks by age group and gender
