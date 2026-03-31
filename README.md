## Credit Portfolio Risk Monitoring Framework

### Description
This project is a SQL-based credit portfolio simulation paired with a Power BI reporting layer for risk monitoring. It focuses on portfolio segmentation, delinquency tracking, expected loss review, and exposure concentration. The reporting structure is meant to reflect how lending portfolios are monitored at a summary level using core credit risk measures.

### Business Objective
Design a monitoring framework that evaluates portfolio risk through:
- Risk tier segmentation
- 30+/60+/90+ delinquency exposure
- Charge-off and loss rate tracking
- Expected loss distribution
- Concentration analysis

### Data Model
The core portfolio structure includes:
- `loans` table
- `risk_tier`
- `fico_band`
- `delinquency_status`
- `charge_off_flag`
- `current_balance`

### Key Metrics
- Loss rate by risk tier
- 30+ delinquency rate
- Expected loss by tier
- Risk-weighted exposure
- Loss concentration percentage

### Insights
- Tier D shows the highest loss rate and expected loss concentration
- Loss concentration is not linear across tiers
- Segmentation remains monotonic, supporting underwriting consistency

### Tools
- SQL
- Power BI
