# Monitoring Plan

## Operational Monitoring
- API latency and error rates
- Data pipeline freshness checks

## Model Monitoring
- Feature drift (PSI/KS checks)
- Prediction distribution shifts
- Calibration drift
- Segment-level fairness indicators

## Alert Thresholds
- High severity: fairness threshold breach, severe drift
- Medium severity: calibration degradation
- Low severity: minor distribution shift

## Response Workflow
1. Alert triggers in monitoring system
2. Risk analyst triages
3. Retraining/recalibration decision
4. Governance sign-off before redeployment
