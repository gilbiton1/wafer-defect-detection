# 🛠️ Semiconductor Wafer Scratch Detection (NI Home Assignment)

This project addresses the task of identifying surface scratches on semiconductor wafers based on die-level tabular data.

The solution was developed as part of a data science home assignment for NI (National Instruments), combining feature engineering, spatial analysis, and robust classification modeling.

---

## 📌 Project Overview

Each wafer contains hundreds of dies, each labeled as Good, Bad, or potentially scratched. The task is to detect dies that are likely scratched based on their spatial properties and neighborhood behavior.

My approach includes:

- 🧱 Feature engineering: spatial coordinates, die types, distance from center, edge detection, and neighborhood context
- 🧠 ML modeling: XGBoost classifier with KFold CV, tuned thresholds, and class imbalance handling
- 📊 Visual inspection: wafer maps showing true vs predicted scratch locations

---

## 🛠️ Tools & Techniques
- Python (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib)
- Custom spatial and neighborhood features
- Class imbalance strategy (threshold tuning instead of SMOTE/oversampling)
- Wafer visualizations for model explainability
---
## 🎯 Highlights
- Designed flexible pipeline for spatial pattern detection using tabular wafer data
- Engineered advanced die-level features such as:
  - Neighbor-based scratch/bad/good counts
  - Edge detection and distance from center
  - Line detection for scratch runs
- Achieved consistent visual alignment with real scratch patterns

## ✅ Conclusions
- The project highlights the importance of domain-driven feature engineering and handling extreme class imbalance.
- Instead of relying on resampling, a threshold-optimization strategy proved more effective for rare defect detection in a highly imbalanced setting.
