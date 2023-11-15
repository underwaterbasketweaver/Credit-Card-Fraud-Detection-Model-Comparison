## README for Credit Card Fraud Detection Project
# Overview
This project focuses on detecting fraudulent credit card transactions using an anonymized dataset of European credit card transactions from 2023, available on Kaggle. Our goal is to evaluate and compare various machine learning models to identify the most effective approach for fraud detection.

# Data Source
The dataset used in this analysis can be found at Kaggle: Credit Card Fraud Detection Dataset 2023.
https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023/

# Objective
Our objective is to assess the effectiveness of different classification models in detecting fraud. The models include K Nearest Neighbors, Random Forest, Logistic Regression, Decision Tree, Support Vector Machine, and Neural Networks.

# Data Description
The dataset contains 568,630 transactions with 28 anonymized features, a 'Class' label indicating fraud (1) or non-fraud (0), and the transaction 'Amount' standardized in Euros.

# Libraries Used
Pandas
NumPy
Matplotlib
Seaborn
Plotly
Scikit-learn
TensorFlow (for Neural Networks)

# Analysis Approach
The analysis includes comprehensive exploratory data analysis (EDA) with visualizations to understand correlations and distributions, followed by data preprocessing, model training, and performance evaluation using metrics such as F1 score and confusion matrices.

# Model Performance
The performance of each model was rigorously evaluated. Random Forest emerged as the top performer, achieving near-perfect classification accuracy. Both the Neural Network and Logistic Regression models were further optimized using RandomizedSearchCV and GridSearchCV, respectively, resulting in significant performance gains.

# Key Findings
Random Forest and Decision Tree classifiers showed exceptional performance.
Logistic Regression, initially the weakest, showed substantial improvement after optimization.
The optimized Neural Network demonstrated the usefulness of hyperparameter tuning.
Conclusion
The Random Forest model stood out as the best model for this specific fraud detection task, showcasing the power of ensemble learning methods in handling complex classification tasks.

# Future Work
Further research could involve deploying the model into a real-time fraud detection system and assessing its performance on a live stream of transaction data.
