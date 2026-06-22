# Obesity Level Classification using Explainable AI (XAI)

## 📌 Project Overview

This project focuses on predicting obesity levels using Machine Learning and explaining model decisions through Explainable Artificial Intelligence (XAI) techniques.

A Random Forest Classifier is trained on obesity-related health and lifestyle data to classify individuals into different obesity categories. To improve transparency and trustworthiness, SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) are used to explain both global and individual predictions.

The project demonstrates how explainable AI can help understand why a machine learning model makes a particular prediction, making it suitable for healthcare, research, and educational applications.

---

## 🎯 Objectives

- Build an obesity classification model using Random Forest.
- Evaluate classification performance.
- Understand the most influential features affecting obesity prediction.
- Generate global explanations using SHAP.
- Generate local explanations using SHAP and LIME.
- Compare SHAP and LIME explanations for the same prediction.
- Demonstrate the importance of explainable AI in healthcare-related applications.

---

## 📊 Dataset

### Obesity Levels Dataset

The dataset contains demographic, lifestyle, dietary, and physical activity information used to classify obesity levels.

### Sample Features

- Gender
- Age
- Height
- Weight
- Family history of obesity
- Frequency of high-calorie food consumption
- Physical activity frequency
- Daily water intake
- Smoking habits
- Alcohol consumption
- Technology usage time
- Transportation mode

### Target Classes

- Insufficient Weight
- Normal Weight
- Overweight Level I
- Overweight Level II
- Obesity Type I
- Obesity Type II
- Obesity Type III

---

## 🛠 Technologies Used

### Programming Language

- Python 3

### Libraries

- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- SHAP
- LIME

### Development Environment

- Google Colab
- Jupyter Notebook

---

## 🔄 Project Workflow

### 1. Data Preprocessing

- Load dataset
- Handle missing values
- Encode categorical features
- Feature selection
- Split dataset into training and testing sets

### 2. Model Training

A Random Forest Classifier is trained using the processed dataset.

```python
RandomForestClassifier(
    n_estimators=100,
    random_state=42
)
```

### 3. Model Evaluation

Performance metrics include:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

### 4. Explainable AI Analysis

The trained model is explained using:

#### SHAP

- Global Feature Importance
- SHAP Summary Plot
- SHAP Dependence Plot
- SHAP Waterfall Plot
- SHAP Force Plot

#### LIME

- Local Prediction Explanation
- Feature Contribution Analysis
- Interactive Explanation Visualization

### 5. SHAP vs LIME Comparison

A side-by-side comparison is performed to understand:

- Feature importance agreement
- Explanation consistency
- Interpretability differences

---

## 📈 Visualizations Generated

### SHAP Visualizations

- SHAP Summary Plot
- SHAP Feature Importance Bar Plot
- SHAP Waterfall Plot
- SHAP Force Plot
- SHAP Dependence Plot

### LIME Visualizations

- LIME Feature Importance Chart
- Interactive Local Explanation

### Comparative Analysis

- SHAP vs LIME Comparison Plot

---

## 🔍 Explainable AI Techniques

### SHAP (SHapley Additive exPlanations)

SHAP is based on game theory and assigns contribution values to each feature.

#### Advantages

- Theoretically grounded
- Consistent explanations
- Supports both global and local explanations
- Ideal for model auditing

---

### LIME (Local Interpretable Model-Agnostic Explanations)

LIME builds a simple surrogate model around a specific prediction.

#### Advantages

- Easy to understand
- Works with any machine learning model
- Provides intuitive rule-based explanations

---

## 📊 Example Analysis

For a given patient/person:

### SHAP Explanation

Shows how each feature pushes the prediction toward or away from obesity.

Example:

- Weight → Strong positive contribution
- Physical activity → Negative contribution
- Family history → Positive contribution

### LIME Explanation

Shows local decision rules such as:

```
Weight > 90 kg
Physical Activity < 2 days/week
Family History = Yes
```

These conditions help explain why the model predicted a particular obesity class.

---

## 📋 Results

The Random Forest model successfully classified obesity levels with strong predictive performance.

Key observations:

- Weight is one of the most influential features.
- Physical activity significantly affects predictions.
- Family history plays an important role.
- SHAP and LIME generally agree on major contributing features.
- SHAP provides more consistent explanations while LIME provides easier-to-understand local rules.

---

## 📚 Educational Outcomes

This project demonstrates:

- Machine Learning Classification
- Healthcare Data Analysis
- Explainable Artificial Intelligence (XAI)
- Model Transparency
- SHAP Interpretability
- LIME Interpretability
- Responsible AI Practices

---

## 🚀 Future Improvements

- Deploy as a Streamlit Web Application
- Add Deep Learning Models
- Compare multiple classifiers
- Generate PDF explanation reports
- Integrate real-time obesity prediction
- Add dashboard visualizations

---

## 👨‍💻 Author

**Kailash**

Machine Learning & Explainable AI Project

---

## ⭐ If you found this project useful

Please consider giving this repository a star on GitHub.
