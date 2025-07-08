# 🧠 Clinical Trial Patient Matching System

This project builds an AI/ML-powered system that **matches patients to relevant clinical trials** based on eligibility criteria like age, gender, medical condition, and more. It simulates a real-world healthcare application used in drug research and preventive care.

---

## 🚀 Problem Statement

The goal is to assist researchers and clinicians by:
- Automatically identifying **suitable clinical trials** for patients
- Using machine learning to evaluate **trial eligibility**
- Ranking and recommending trials using **criteria matching and scoring**

---

## 🔧 Skills Demonstrated

| Area            | Description |
|-----------------|-------------|
| 🧠 AI/ML         | Random Forest Classifier for predicting trial eligibility |
| 🎯 Criteria Scoring | Patient–Trial match scoring based on simulated features |
| 📊 Ranking Engine | Sorted recommendations based on match score |
| 🔍 Evaluation     | Accuracy, precision, recall, confusion matrix |
| 🧱 Modular Design | Separation of scoring, matching, and ML modeling |
| 🧬 Preventive Care | Simulated risk detection for lifestyle conditions |

---

## 🧪 Dataset

- **300 rows × 100 columns** synthetic patient data
- Each row = 1 patient’s health record (features)
- Label (`0` or `1`): whether the patient qualifies for a trial
- Matching criteria:  
  ```python
  y = ((feature_1 + feature_2 + feature_3) > 1.5).astype(int)


🛠️ Tools & Libraries
Python, NumPy, Pandas

scikit-learn

Matplotlib, Seaborn

Google Colab (recommended)

🧬 Project Architecture
java
Copy
Edit
Patient Profile (300 × 100)
        ↓
Eligibility Criteria Logic (Similarity + Scoring)
        ↓
Match Label (0/1)
        ↓
Train/Test Split
        ↓
Random Forest Classifier
        ↓
Prediction + Evaluation + Ranking
📈 Model Performance
✅ Accuracy Score: 0.90

📊 Classification Report:

markdown
Copy
Edit
              precision    recall  f1-score   support

           0       0.90      1.00      0.95        36
           1       0.00      0.00      0.00         4

    accuracy                           0.90        40
   macro avg       0.45      0.50      0.47        40
weighted avg       0.81      0.90      0.85        40
📉 Confusion Matrix:

lua
Copy
Edit
[[36  0]
 [ 4  0]]
⚠️ Note: The model struggles with minority class (few positive matches).
You can improve this with SMOTE, class weights, or a larger dataset.

📊 Visualizations
Confusion Matrix Heatmap

Feature Importance Bar Chart (Top 10 predictors)

💡 Future Improvements
Simulate more realistic trial data (e.g., age, gender, disease type)

Add exclusion criteria logic

Use XGBoost or Neural Networks for learning complex rules

Deploy as a Streamlit or Flask Web App

Integrate real datasets from ClinicalTrials.gov or Kaggle

📂 Project Structure
bash
Copy
Edit
📁 clinical_trial_matcher/
│
├── clinical_trial_matcher.ipynb       # Google Colab Notebook
├── README.md                          # Project Overview
├── trial_data.csv (optional)          # Exported dataset
└── model.pkl (optional)               # Saved trained model
👨‍⚕️ About Preventive Healthcare
This project aligns with the mission of preventive health by helping:

Patients discover trials for early intervention

Researchers find the right participants quickly

Data scientists build real-world healthcare solutions

📜 License
This project is open-source and available under the MIT License.

🙋‍♂️ Author
Anirudh
Passionate about healthcare, AI, and real-world problem solving.
