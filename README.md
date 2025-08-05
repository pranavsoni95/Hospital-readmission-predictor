
# 🏥 Project Title: Hospital Readmission Risk Prediction

## 🧾 Brief One Line Summary
Predicting hospital readmissions using machine learning (Random Forest) and visualizing key patterns with Power BI.

---

## 📖 Overview
Hospital readmissions are a critical metric for evaluating healthcare quality and controlling costs. This project leverages machine learning to predict whether a patient is likely to be readmitted within 30 days of discharge and visualizes key insights via a Power BI dashboard for healthcare decision-makers.

---

## ❗ Problem Statement
Unplanned hospital readmissions are costly and often avoidable. Hospitals face pressure to reduce readmission rates, both for improving patient care and avoiding penalties. Predicting readmissions early allows medical professionals to proactively intervene.

---

## 📊 Dataset
- **Source:** Publicly available dataset from the UCI Machine Learning Repository
- **File:** `Prediction_Data.xlsx`
- **Target Column:** `readmitted` (`<30` = Readmitted, `NO`/`>30` = Not Readmitted)
- **Records:** ~98,000
- **Features:** Demographics, diagnoses, treatments, lab results, medications

---

## 🧰 Tools and Technologies
- **Languages:** Python, SQL
- **Libraries:** Pandas, NumPy, Scikit-learn, Imbalanced-learn (SMOTE), Seaborn, Matplotlib
- **Visualization:** Power BI
- **Model:** Random Forest Classifier
- **Model Serialization:** joblib

---

## ⚙️ Methods
1. Data Cleaning and Preprocessing
2. Label Encoding for categorical variables
3. Handling class imbalance using **SMOTE**
4. Train-test split using **stratified sampling**
5. Model training using **Random Forest**
6. Model evaluation using **confusion matrix** and **classification report**
7. Predictions saved to CSV for Power BI
8. Power BI dashboard built for insights and presentation

---

## 💡 Key Insights
- Age group `70–80` had the highest number of readmissions.
- Patients with longer **time in hospital** tend to have higher readmission likelihood.
- Insulin type and A1C results strongly influence the prediction outcome.
- Readmission rates vary significantly by race and gender.

---

## 📈 Dashboard/Model/Output
- 📌 **Model Accuracy:** ~84%
- 📊 **Power BI Dashboard Includes:**
  - Total patients, predicted patients, and readmission rate
  - Readmission count by age, race, gender, A1C result, insulin usage, and time in hospital
  - Interactive filters (insulin, gender)
  - Dynamic table with patient predictions

---

## ▶️ How to Run this project?

### 🔧 Step-by-step:
1. Clone the repository
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook:
    - Loads and preprocesses data
    - Trains Random Forest model
    - Outputs predictions to `ReadmissionPredictions.csv`
4. Open Power BI and connect it to the CSV
5. Design dashboard based on fields like `Predicted_Readmission`, `age`, `gender`, etc.

---

## 📌 Results & Conclusion
The model shows strong performance in predicting hospital readmissions, especially for the majority class. SMOTE helped improve recall for minority class (`<30` readmissions). The Power BI dashboard complements the prediction by offering an intuitive, data-driven storytelling interface.

---

## 🚀 Future Work
- Add SHAP values for model explainability
- Deploy the model using Streamlit for real-time scoring
- Connect Power BI to live database for up-to-date dashboards
- Integrate more clinical variables like medications and comorbidities

---

## 👨‍💻 Author & Contact
**Pranav Soni**  
📫 Email: pranavsoni9596@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/pranav-soni-826a43222/)  
🐙 [GitHub](https://github.com/pranavsoni95)

---

⭐ *If you found this project helpful, give it a star and share it with others!*
