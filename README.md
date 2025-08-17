# Predicting Student Stress Levels: A Data-Driven Analysis

This repository contains the code and findings for the Capstone Project for the Student Developer Initiative, focusing on predicting student stress levels using machine learning.

---

## 📋 Project Overview

### Background
Student stress is a critical issue in modern education, impacting academic performance, mental health, and overall well-being. This project moves beyond general assumptions by applying a data analytics methodology to identify the specific factors that are most predictive of high stress levels.

### Objective
The primary objective is to build and validate a machine learning model that can accurately predict a student's stress level (Low, Medium, or High) and to use this model to uncover the key drivers of stress among various psychological, social, and physiological factors.

### Dataset
The analysis is based on the **Student Stress Factors** dataset from Kaggle, which contains survey data from 1100 students.
* **Link**: [Kaggle](https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets?select=StressLevelDataset.csv)

---

## ⚙️ Analysis Process

The project followed a systematic data science workflow to ensure robust and reliable results:

1.  **Data Exploration & Visualization**: The dataset was first analyzed to understand its structure and identify initial trends. Boxplots were used to visualize the relationship between individual factors and the reported stress level.

2.  **Feature Selection**: To isolate the most predictive features, a multi-faceted approach was employed, using three distinct methods: **Random Forest Importance**, **ANOVA F-test**, and **Recursive Feature Elimination (RFE)**. This process narrowed down the original 20+ factors to the 7 most influential predictors.

3.  **Model Training & Tuning**: Several classification models were trained and compared. The **Random Forest** model was selected for its high performance and was further optimized using **GridSearchCV** to find the best hyperparameters, resulting in a final model with 86% accuracy.

4.  **In-depth Interpretation**: The final model was analyzed using advanced techniques to understand its logic. **ROC/AUC curves** were generated to get a nuanced measure of its classification power, and **SHAP (SHapley Additive exPlanations)** was used to explain the "why" behind its predictions and uncover feature interactions.

---

## 💡 Insights & Findings

The analysis yielded several unique and actionable insights:

* **Top Predictors**: The final model identified a mix of physiological, academic, and psychological factors as the most powerful predictors of stress. The top factors include **Blood Pressure**, **Sleep Quality**, **Academic Performance**, and **Anxiety Level**.

* **The Hidden Amplifier**: A critical interaction effect was discovered between **bullying** and **sleep quality**. The negative impact of bullying on stress is significantly **amplified** when a student also suffers from poor sleep. This highlights that key stress factors do not act in isolation.

* **High Model Reliability**: The final tuned model is highly reliable, achieving **86% accuracy** and an outstanding **AUC score of over 0.98**. This confirms its strong ability to distinguish between low, medium, and high-stress students.

---

## ✅ Conclusion & Recommendations

### Conclusion
Student stress is a predictable and multifaceted issue. This project successfully developed a reliable model that confirms stress is driven by an interplay of physiological, social, and psychological factors.

### Actionable Recommendations
Based on the insights, the following concrete recommendations are proposed for educational institutions:

1.  **Prioritize Sleep Hygiene Education**: As good sleep acts as a protective buffer, providing resources on healthy sleep habits can be a high-impact wellness initiative.
2.  **Strengthen Anti-Bullying Initiatives**: Given its role as a major stress amplifier, especially when combined with poor sleep, anti-bullying programs are critical.
3.  **Promote Social Support Networks**: Foster environments and programs that strengthen peer and faculty social support systems to build student resilience.

---

## 🤖 AI Support Explanation

This project leveraged AI as a collaborative tool to enhance the analytical workflow:

* **High-Level Planning**: **IBM Granite** was used at the project's outset to define the high-level steps for the classification task.
* **Detailed Analysis & Implementation**: **IBM Granite** was used for brainstorming advanced analytical steps, generating Python code for complex libraries (`GridSearchCV`, `SHAP`, `Gradio`), debugging technical errors, and interpreting complex visualizations.
