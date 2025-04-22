# 🚗 Road-Accident-Severity-Prediction-A-Seattle-Case-Study

## 📘 Overview

This project is part of the IBM Coursera Applied Data Science Capstone and focuses on analyzing and predicting the **severity of car collisions** in Seattle from 2004 to 2020. The dataset includes environmental and situational factors surrounding each accident, such as road condition, light condition, and weather. Using various machine learning models, this project aims to identify patterns and help stakeholders develop strategies to reduce accident severity.

---

## 📊 Dataset Information

- **Source**: Seattle Department of Transportation (via Seattle Open Data Portal)
- **Timeframe**: 2004 – August 2020
- **Format**: CSV
- **Records**: ~221,000
- **Features**: 40 attributes including weather, road, location, and severity code
- **Target Variable**: `SEVERITYCODE`
    - 0: Unknown  
    - 1: Property damage only  
    - 2: Minor injury  
    - 2b: Serious injury  
    - 3: Fatality

---

## 🧹 Data Preprocessing

- Removed missing or irrelevant data (especially `SEVERITYCODE = 0` or `Unknown`)
- Combined severity labels into 2 categories:
  - **Property Damage Only**
  - **Injury (Minor/Serious/Fatal)**

---

## 📈 Exploratory Data Analysis (EDA)

EDA was performed to investigate:
- Distribution of severity types
- Effect of weather, road, and light conditions on collisions
- Location-based collision trends (block vs. intersection)

Key Findings:
- Most collisions occur during **daylight**, in **clear weather**, and on **dry roads**
- Human factors like distraction and fatigue are likely significant contributors

---

## 🤖 Machine Learning Models

The following classification models were implemented:

| Model              | Training Accuracy | Testing Accuracy |
|-------------------|-------------------|------------------|
| K-Nearest Neighbors (KNN) | 66.95%            | 67.00%           |
| Decision Tree             | 69.70%            | 69.59%           |
| Support Vector Machine (SVM) | 69.69%        | 69.58%           |
| Logistic Regression       | 69.57%            | 69.49%           |

All models performed similarly with an accuracy of around 69%.

---

## 🧠 Conclusions

- Most accidents occur not due to poor environmental conditions but likely due to **human error**
- The models built can predict accident severity based on external conditions with ~69% accuracy
- Insights from this study can help **road safety planners**, **emergency responders**, and **policymakers** reduce accident impact

---

## 🎯 Target Audience

- City/Road Planners  
- Emergency Services  
- Police Departments  
- General Public  
- World Road Associations

---

## 📌 Future Work

- Include driver behavior data if available (e.g., distraction, intoxication)
- Use deep learning models to improve predictive accuracy
- Implement real-time severity prediction systems for smart cities

---

## 📂 Files in Repository

- `Collision_Severity_Analysis.ipynb`: Jupyter Notebook containing full analysis
- `collision_data.csv`: Original dataset
- `README.md`: Project overview and documentation
- `visualizations/`: Folder for saved graphs and plots

---

## 👨‍💻 Author

**Nandan Choudhary**  
IBM Applied Data Science Capstone  
Date: October 12, 2020
