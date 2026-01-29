# Industrial SCADA Data Analysis for Wind Turbine Fault Detection & Operational Insights

This project focuses on analyzing real-world industrial SCADA data from wind turbines to detect early fault signals and translate technical analysis into actionable maintenance insights.

The work is structured into three phases, progressing from raw data understanding to a business-oriented dashboard for predictive maintenance.

---

## Phase 1 – Data Understanding & Exploratory Analysis

The goal of this phase was to build a solid understanding of normal turbine behavior and data reliability, forming the foundation for anomaly detection.

Key activities:
- Worked with time-based, continuous SCADA sensor data
- Focused on a single turbine (asset_id = 0) to establish a normal operating baseline
- Explored sensor distributions, correlations, and overall data quality
- Verified physical relationships such as wind speed versus power output
- Observed that anomalies in industrial systems usually appear as gradual drifts rather than sudden failures

---

## Phase 2 – Anomaly Detection & Early Warning Signals

The objective of this phase was to detect early deviations from normal operation using operational patterns.

Key activities:
- Built a power curve baseline using wind speed and active power
- Calculated rolling statistics to capture local behavior changes
- Defined upper and lower operational limits
- Identified anomalies as deviations from expected power output
- Classified operational states into:
  - **Normal**
  - **Watch** (early warning)
  - **Alert** (high-risk deviation)

**Key insight:**  
Most critical faults do not start as alerts. They first appear in the *Watch* stage, where early intervention can prevent unplanned downtime.

---

## Phase 3 – Business View & Predictive Maintenance Dashboard

The focus of this phase was to translate analytical results into operational and business impact.

Key activities:
- Prepared a clean, minimal dataset for visualization
- Designed an interactive Power BI dashboard, including:
  - Operational KPIs
  - Power curve anomaly visualization
  - Early warning timeline
  - Condition-based maintenance indicators
- Estimated business impact using a simple, explainable model:
  - Potential downtime saved
  - Availability improvement target

**Business perspective:**  
Instead of routine or reactive maintenance, the dashboard supports
**condition-based and predictive maintenance**, enabling earlier and more informed decisions.

---

## Dashboard Highlights
- Early detection of deviations under normal wind conditions
- Clear separation between normal operation and warning states
- Estimated impact metrics for maintenance decision-makers

---

## Tools & Technologies
- Python (Pandas, NumPy, Matplotlib)
- Jupyter Notebooks
- Power BI
- GitHub for project versioning

---

## Final Note
This project demonstrates a complete analytics pipeline:
from raw industrial SCADA data to decision-ready insights, with a strong focus on real-world applicability and business value.
