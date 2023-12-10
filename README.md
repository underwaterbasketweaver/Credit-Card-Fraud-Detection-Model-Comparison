## README for Credit Card Fraud Detection Project
# Overview
This project focuses on detecting fraudulent credit card transactions using an anonymized dataset of European credit card transactions from 2023, available on Kaggle. My goal is to evaluate and compare various machine learning and artificial intelligence models to identify the most effective approach for fraud detection.  

Credit Card Fraud accounts for a small % of transactions, under a tenth of a percent, but due to the volume of transactions this still adds up to nearly 2 billion euros annually, in addition to the over half a billion GBP lost to fraud annually. This does not necessairly cover the full cost of the fraud by the time the process in complete born by the various parties involved.

Accuratly detecting and flagging suspicious transactions for prompt customer review is an essential part of effectivley operating any card based payment service or network. AI and ML methods offer the most effective way of doing this, and quickly detecting fraud is essential to mitigate the costs.

# Data Source
The dataset used in this analysis can be found at Kaggle: Credit Card Fraud Detection Dataset 2023.
https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023/

# Objective
My objective is to assess the effectiveness of different classification models in detecting fraud. The models include K Nearest Neighbors, Random Forest, Logistic Regression, Decision Tree, Support Vector Machine, and Neural Networks.

# Data Description
The dataset contains 568,630 transactions with 28 anonymized features, a 'Class' label indicating fraud (1) or non-fraud (0), and the transaction 'Amount' standardized in Euros. Transactions are evenly split between fradulent and non fradulent transactinos.  Unfortunately I have yet to find additional data.

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
Various ensamble techniques were employed  - these are basically models that allow a combination of the best performing of the other models to vote and collectivley decide wheather or not a transaction is fraud.
The best performing were custom weighted ensambles.

Conclusion
The customized ensamble models offered the best F1 accuracy, with 1 model even correctly detecting 100% of instances of fraud, at the cost of a significant increase in false negatives.  

# Future Work
Further research could involve obtaining more data and testing model performance and further optimizations
