# Data Science Methodology: A Case Study
# 🎗️ Predict the Diagnosis of a Breast Cancer Patient

This Project is a case study of my project Breast Cancer Diagnosis Prediction Model you can check out the project [Here](https://github.com/JayshreeMishra/Data_Science_Projects/tree/main/Project%203%20-%20Cancer%20Prediction)

## 🧠 Business Understanding

This project begins at the **Business Understanding** stage — the foundational step of the Data Science Methodology. 

Assuming the role of a data scientist, I focused on translating a critical healthcare question into a data science problem:  
> **Can we automatically predict the diagnosis of a breast cancer patient using computed features from cell nucleus images?**

This question reflects a high-impact classification problem with real-world significance. To address it, I followed the structured pipeline of the data science lifecycle — from identifying analytical goals to evaluating a working model.

---

## 🔍 1. Analytical Approach

I approached this as a **predictive modeling** task. The objective was to build a classification model that could predict whether a breast tumor is benign or malignant, based on quantifiable features extracted from digitized cell nucleus images.

---

## 📋 2. Data Requirements

To meet this objective, the model requires structured data describing the physical characteristics of the cell nuclei observed in breast mass tissue. These include:
- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Concave points
- Symmetry
- Fractal dimension

These features act as **independent variables**, while the diagnosis (benign or malignant) is the **target variable**.

---

## 📦 3. Data Collection

The dataset used was the publicly available **Breast Cancer Wisconsin Diagnostic Dataset**. It contains:
- 30 numerical features computed from cell nucleus images
- A diagnosis label for each patient sample
- No personally identifiable information, ensuring ethical usage

---

## 🔍 4. Data Understanding & Preparation

During the **data understanding** phase, I examined the structure and distributions of the input features and target variable.  
Key observations included:
- The target variable (`diagnosis`) is binary: *B* (benign) or *M* (malignant).
- Each feature (e.g., `radius_mean`, `concavity_mean`, `symmetry_worst`) represents a measured property of the cell nuclei.

In the **data preparation** stage, I performed the following steps:
- Verified class balance across the diagnosis labels
- Checked for and confirmed absence of missing values
- Removed duplicates to ensure data integrity
- Normalized features where needed to standardize input for modeling

---

## 🤖 5. Modeling & Evaluation

To classify the tumors, I trained a **Logistic Regression** model. This model was chosen for its interpretability and suitability for binary classification tasks.

**Evaluation** included:
- Splitting the dataset into training and testing sets (80/20 split)
- Measuring performance using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Interpreting coefficients to understand which features contributed most to the classification


  
