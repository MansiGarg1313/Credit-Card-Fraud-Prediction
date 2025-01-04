## Credit Card Fraud Prediction

### Overview

This project aims to predict fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced, with a small percentage of transactions being fraudulent. The focus is on creating a robust model to accurately identify fraudulent transactions while minimizing false positives.

### Dataset

The dataset used in this project contains anonymized credit card transaction data with the following key characteristics:

Features: 28 numerical features resulting from a PCA transformation (V1 through V28).

Other Variables:

Time: Seconds elapsed between the transaction and the first transaction in the dataset.

Amount: Transaction amount.

Class: Target variable where 1 indicates fraud and 0 indicates non-fraud.

### Dataset Challenges

Imbalance: Only 0.172% of transactions are fraudulent.

Anonymized Data: Features are anonymized for confidentiality, making domain-specific feature engineering challenging.

### Methodology

Data Preprocessing:

Standardization of the Amount and Time features.

Handling imbalanced data using oversampling (SMOTE) and undersampling techniques.

Splitting the dataset into training and testing sets.

### Exploratory Data Analysis (EDA):

Distribution of fraudulent vs. non-fraudulent transactions.

Correlation analysis to identify feature interactions.

Visualizations of transaction amounts and time distributions.

### Modeling:

Multiple classification algorithms implemented, including:

Logistic Regression

Random Forest

Gradient Boosting (e.g., XGBoost, LightGBM)

Performance metrics used:

Precision, Recall, F1-score, ROC-AUC.

### Evaluation:

Comparison of models based on their ability to detect fraudulent transactions.

Focus on minimizing false negatives while keeping false positives manageable.

### Results

Models were evaluated using a combination of confusion matrices, precision-recall curves, and ROC-AUC scores.

Ensemble methods like Random Forest and Gradient Boosting showed superior performance compared to baseline models like Logistic Regression.

### Tools and Libraries

Python 3.8+

Libraries:

pandas

numpy

scikit-learn

imbalanced-learn

matplotlib

seaborn

XGBoost


### Acknowledgements

The dataset is publicly available on Kaggle.
