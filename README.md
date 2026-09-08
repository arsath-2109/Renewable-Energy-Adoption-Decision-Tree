# ♻️ Renewable Energy Adoption Prediction

## 📌 Project Overview

This project uses **Machine Learning** to predict whether a renewable energy system will be **adopted or not adopted** based on environmental, energy, and economic factors.

A **Decision Tree Classifier** is trained using four input features:

- Carbon Emissions
- Energy Output
- Renewability Index
- Cost Efficiency

The model is evaluated using accuracy, confusion matrix, and classification report. The trained model is also saved as a `.pkl` file for future use.

---

## 🎯 Problem Statement

Renewable energy adoption depends on several factors, including environmental impact, energy production, renewable potential, and cost efficiency.

Manually analyzing these factors can be difficult. This project develops a Machine Learning model that predicts renewable energy adoption based on these parameters.

---

## 💡 Proposed Solution

A **Decision Tree Classification** algorithm is used to classify renewable energy systems into two categories:

- **1 → Adoption**
- **0 → Non-Adoption**

The model learns patterns from the training dataset and predicts the adoption status of previously unseen data.

---

## 🧠 Machine Learning Algorithm

### Decision Tree Classifier

A Decision Tree is a supervised Machine Learning algorithm used for classification and regression tasks.

In this project, the tree is limited to a maximum depth of **3** to reduce the possibility of overfitting.

```python
model = DecisionTreeClassifier(
    max_depth=3,
    random_state=42
)
