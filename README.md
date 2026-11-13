# Influencer Fraud Detection

A Python-based Machine Learning project designed to identify potentially fraudulent social media influencer profiles using engagement metrics, anomaly detection, and risk scoring.

## Project Overview

The project analyzes influencer profile data to identify unusual engagement patterns and suspicious account behavior. It aims to help marketing teams prioritize influencer profiles for manual verification before approving campaigns.

## Objectives

- Analyze influencer profile and engagement data.
- Perform data cleaning and Exploratory Data Analysis (EDA).
- Engineer meaningful engagement-related features.
- Apply unsupervised machine learning algorithms for anomaly detection.
- Generate risk scores and verification recommendations.

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Jupyter Notebook
- Isolation Forest
- Local Outlier Factor (LOF)

## Project Workflow

1. Data collection and quality checks.
2. Exploratory Data Analysis (EDA).
3. Feature engineering using engagement metrics.
4. Anomaly detection using Isolation Forest and LOF.
5. Risk score generation and risk categorization.
6. Model evaluation and CSV export.

## Machine Learning Approach

Isolation Forest and Local Outlier Factor (LOF) were explored to identify potentially suspicious influencer profiles.

A percentile-based 0–100 anomaly risk score was developed to categorize profiles into:

- Low Risk
- Medium Risk
- High Risk

The categories are linked to suggested verification actions, including Basic Check, Manual Review, and Detailed Verification.

**Note:** The anomaly risk score represents relative anomaly severity, not the probability that an influencer is fraudulent.

## Model Evaluation

**Main Validation Experiment**

The improved model was evaluated on a 200-profile simulated reference-labeled sample.

- Precision: 88.89%
- Recall: 36.92%
- Risk Threshold: 90

**Supplementary BON Dataset Experiment**

- Precision: 94.34%
- Recall: 3.57%
- Flagged Profiles: 106

The BON experiment demonstrates a precision-focused result with low recall.

## Project Files

- `INTERNSHIP.ipynb` – Main Jupyter Notebook.
- `INTERNSHIP.py` – Python script.
- `Influencer-Fraud Detection.csv` – Main influencer dataset.
- `Model validation.csv` – Reference validation sample.
- `bon_dataset.csv` – Supplementary BON dataset.
- `influencer_fraud_final.csv` – Final influencer risk-score output.
- `Influencer_Fraud_Detection_Final_Report.pdf` – Project report.

## Limitations

- The 200 reference labels are simulated and not independently human-verified.
- The model may miss fraudulent profiles because recall is limited.
- The risk score should not be interpreted as a calibrated fraud probability.
- The system is a screening prototype and requires manual verification before business decisions.

## Future Improvements

- Improve precision-recall balance.
- Add model explainability.
- Evaluate performance across influencer segments.
- Develop reusable scoring pipelines and automated tests.

## Author

**Yashdeep**

Machine Learning | Data Analysis | Python
