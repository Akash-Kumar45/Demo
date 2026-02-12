# Model Card: LifeShield Mortality Risk Predictor v2.3.0

## Model Details
- Model Type: Gradient Boosted Trees
- Version: 2.3.0
- Owner: Risk Analytics Team
- Status: Active

## Intended Use
Assist life underwriting by estimating short-term mortality risk. Not intended for fully automated approvals.

## Training Data
- Time window: 2018-2024
- Population: Individual life insurance applicants
- Labels: 1-year mortality outcome proxy from claims records

## Key Performance Metrics
- AUC: 0.84
- Precision (High-risk band): 0.71
- Recall (High-risk band): 0.68
- Brier score: 0.16

## Validation
- Temporal split validation
- Out-of-time holdout test
- Stability check across policy product types

## Fairness and Bias Checks
- Segment checks by gender and age band
- No segment should exceed predefined error disparity thresholds
- Escalation required if threshold breached

## Limitations
- Sensitive to data quality and coding changes in source systems
- May underperform for underrepresented subpopulations
- Requires periodic recalibration

## Governance Controls
- Independent model validation required before major releases
- Change log and approval required for feature/schema changes
- Monitoring alerts routed to Risk Governance team
