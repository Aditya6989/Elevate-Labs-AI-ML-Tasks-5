🩺 Heart Disease Prediction with Decision Tree & Random Forest
📁 Project Overview
This project uses a heart disease dataset to build and evaluate machine learning models for predicting the presence of heart disease. We explore Decision Trees and Random Forests, visualize results, interpret feature importance, and evaluate models using cross-validation.

📊 Dataset
File: heart.csv
Source: UCI Heart Disease Dataset
Target column: target (1 = disease, 0 = no disease)
Features include:

age, sex, cp (chest pain type)

trestbps (resting blood pressure), chol (cholesterol)

fbs (fasting blood sugar), restecg, thalach (max heart rate)

exang (exercise-induced angina), oldpeak, slope, ca, thal

✅ Steps Performed
1. Train a Decision Tree Classifier
Built a model using scikit-learn

Visualized the tree with plot_tree()

2. Analyze Overfitting & Control Depth
Compared training and test accuracy across tree depths

Identified overfitting and optimal depth

3. Train a Random Forest
Built a more robust model with multiple trees

Compared accuracy with single tree model

4. Interpret Feature Importances
Visualized the most important features contributing to prediction

5. Evaluate with Cross-Validation
Used k-fold cross-validation for reliable performance estimation

📌 Requirements
Python 3.x

pandas, numpy

scikit-learn

matplotlib

Install requirements:

bash
Copy
Edit
pip install pandas numpy scikit-learn matplotlib
📈 Results
Decision Tree Accuracy (depth-tuned): ~82%

Random Forest Accuracy: ~85–88%

Top Features: cp, thalach, oldpeak, ca, thal

📚 Key Concepts
Decision Trees and their interpretability

Entropy & Information Gain

Overfitting and depth pruning

Bagging and Random Forests

Feature importance interpretation

🔍 Visualization Examples
Tree plots for interpretability

Feature importance bar charts

Accuracy vs. Tree Depth graph
