# Machine-Learning

# 🍷 Wine Quality Prediction

This project aims to predict the quality of red wine using machine learning models based on various physicochemical features in the dataset. The models classify whether the wine is of **good quality (≥7)** or not.

---

## 📌 Problem Statement & Objectives

The goal of this project is to build machine learning models that can classify red wines as *good* or *not good* based on various chemical attributes like acidity, alcohol, sulfur dioxide, etc. This classification helps wineries ensure quality control and identify potential quality wines early.

**Objectives:**
- Explore and understand the wine quality dataset.
- Perform data visualization and statistical analysis.
- Preprocess data and transform it for model input.
- Apply and compare multiple machine learning models.
- Evaluate models to select the best-performing one.

---

## 📊 Data Acquisition

- **Dataset**: [UCI Red Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)
- **Format**: CSV
- **Features**: 11 physicochemical variables (e.g., pH, alcohol, citric acid, etc.)
- **Target Variable**: `quality` (score between 0 and 10)

---

## 🧹 Data Preprocessing

- Checked for null values.
- Basic statistical analysis using `describe()` and `groupby()`.
- Created a new binary target variable:
  ```python
  df['goodquality'] = [1 if x >= 7 else 0 for x in df['quality']]

## 📈 Data Analysis & Visualization

Countplots for features like quality, pH, alcohol, sulphates, etc.

KDE Plot and Histogram for distribution analysis.

Box Plot and Violin Plot for feature spread and quality relationships.

Heatmap for feature correlation.

Pairplot to analyze bivariate distributions.

Feature Importance from Random Forest to identify top contributing factors.

## 🤖 ML Techniques Used

Trained and evaluated the following models:

Model	Accuracy Score
Random Forest	89.3%
K-Nearest Neighbors	87.2%
Logistic Regression	87.0%
Support Vector Classifier	86.8%
Decision Tree	86.4%
Gaussian Naive Bayes	83.3%

## 🧪 Training & Evaluation

Train/Test Split: 70% training, 30% testing

Metrics:

Accuracy Score

Confusion Matrix

Best Model: Random Forest Classifier

## Conclusion

Random Forest outperformed other models in predicting wine quality.

Alcohol and volatile acidity were among the most important features.

Visualizations and correlations help understand the dataset and guide feature selection.
