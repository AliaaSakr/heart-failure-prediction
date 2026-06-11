# Heart Failure Risk Prediction
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![SHAP](https://img.shields.io/badge/XAI-SHAP-blueviolet?style=for-the-badge)
##  Project Overview
A production-focused machine learning classification project designed to predict heart failure patient outcomes. Because this is a clinical use case, the project prioritizes model interpretability and minimizing false negatives.

## Key Methodologies & Workflow
* **Clinical Metric Optimization:** Tuned the classification threshold to strictly optimize for **Recall**, ensuring high-risk patients are not missed.
* **Explainable AI :** Integrated **SHAP (SHapley Additive exPlanations)** to visually break down feature importance and explain individual patient risk factors.
* **Production Readiness:** Structuring code for deployment and implementing a framework for **data drift monitoring** to maintain long-term model reliability.

* ## Results & Key Takeaways
* **Clinical Metric Optimization:** Successfully shifted the model's decision threshold to maximize **Recall/Sensitivity**. This prioritized capturing true positive heart failure risks, reducing dangerous false negatives to a minimum.
* **Actionable Model Interpretability:** Integrated SHAP summary plots to move away from "black-box" machine learning. The global analysis revealed that Serum Creatinine, Ejection Fraction and Age were the most heavily weighted features driving risk predictions.
* **Local Explainability:** Developed a framework using SHAP force plots to explain *individual* patient risk profiles, demonstrating how a data product can provide doctors with transparent, case-by-case reasoning.
* **Production & Drift Strategy:** Designed a blueprint for deployment that includes data drift monitoring. This ensures that if the incoming patient demographics shift over time, the model triggers a retraining alert to prevent performance degradation in production.
