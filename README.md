# Data-Bootcamp-Final-Project
# Predicting High-Rated Apps on the Google Play Store

This project uses machine learning to classify whether an app on the Google Play Store is highly rated (rating ≥ 4.5) based solely on its metadata. The goal is to identify which features are most predictive of user satisfaction and to build interpretable models that can inform developers and product strategists.

---

## Research Questions

- What metadata features are most correlated with high user ratings?
- How well can different models classify high-rated apps based on structured data?
- What practical insights can developers gain from feature importance?

---

## Models Used

- Logistic Regression (Baseline)
- K-Nearest Neighbors (Tuned)
- Decision Tree (Depth = 9)
- Random Forest (Best Overall)

All models were built using a standardized preprocessing pipeline with scaling, encoding, and cross-validation.

---

## Key Findings

- **Random Forest** delivered the best overall performance (Accuracy: 86.1%, F1 Score: 0.48).
- **Rating Count** and **Install metrics** are the strongest predictors of app quality.
- Features like pricing, ads, and category had lower individual impact but remain actionable for strategy.

---

## Repository Contents

- `Dataset.ipynb`: Script to download and prepare the original dataset
- `final_eda.ipynb`: Exploratory Data Analysis and initial data cleaning
- `final_modeling.ipynb`: Feature engineering, modeling pipeline, and evaluation
- `Final Project Report.pdf`: Written report with key findings, model insights, and strategic implications

---

## Dataset and Sampling

The analysis was performed on a **10% stratified sample** of a cleaned dataset containing over 525,000 apps. This sampling was used to reduce computational load while preserving class balance. Future work may apply models to the full dataset for improved recall.

---

## Next Steps

- Extend to full dataset and test resampling strategies for imbalance
- Incorporate user-generated features like reviews and text sentiment
- Explore advanced models (e.g., XGBoost, LightGBM)
- Compare results with Apple App Store data for generalization

---

## How to Run

1. Clone or download this repository to your local machine.
2. Open `Dataset.ipynb` to download the raw dataset.
3. After downloading, upload the dataset into both `final_eda.ipynb` and `final_modeling.ipynb`.
4. Run all cells in `final_eda.ipynb` to perform data cleaning and exploration.
5. Proceed to `final_modeling.ipynb` to run the modeling pipeline and view results.
6. Review outputs, charts, and performance metrics to interpret the findings.

---

