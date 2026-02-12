# Evaluation Summary (v2.3.0)

## Test Setup
- Temporal holdout: last 6 months
- Baseline: logistic regression benchmark
- Candidate: gradient boosted trees

## Results
- Candidate outperformed baseline on AUC and calibration
- High-risk precision improved by 9%
- Stable performance across major product segments

## Residual Risks
- Drift observed in lab summary feature distributions
- Slight degradation in one age segment in Q4

## Action Items
- Add monthly drift alert for top 10 features
- Recalibrate probability bins quarterly
- Expand fairness checks to smoking-status subgroups

