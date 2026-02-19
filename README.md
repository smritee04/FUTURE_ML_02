FUTURE_ML_02 – Support Ticket Classification & Priority Prediction

Domain: Machine Learning
Track Code: ML
Internship ID: FIT/JAN26/ML5123

Task Overview

This project focuses on building an intelligent system that automatically classifies customer support tickets into categories and predicts their priority level using Natural Language Processing (NLP) and Machine Learning.

It was completed as part of the Machine Learning Internship at Future Interns, with the goal of reducing manual workload and improving support response efficiency.

Dataset

Name: Customer Support Tickets Dataset

Source:
https://www.kaggle.com/datasets/suraj520/customer-support-ticket-dataset

The dataset contains real-world customer support scenarios across multiple departments.

Tools & Libraries

Language: Python 3.x
Environment: Jupyter Notebook / VS Code

Libraries Used:

Pandas & NumPy → Data handling

NLTK → Text preprocessing and lemmatization

Scikit-learn → TF-IDF, Logistic Regression, Evaluation

Matplotlib & Seaborn → Visualization

Regex (re) → Text cleaning

Methodology
🔹 Data Preprocessing

Combined Ticket Subject + Ticket Description into a single text column

Converted text to lowercase

Removed special characters using regex

Removed stopwords (NLTK)

Applied lemmatization

🔹 Feature Engineering

TF-IDF Vectorization

max_features = 5000

🔹 Model Training

Two separate models were trained:

1️.Ticket Category Prediction Model

Target: Ticket Type

Algorithm: Logistic Regression

2️.Ticket Priority Prediction Model

Target: Ticket Priority

Algorithm: Logistic Regression with class_weight='balanced'

🔹 Train-Test Split

80% Training

20% Testing

Random State = 42

Model Evaluation

Evaluation metrics used:

Precision

Recall

F1-Score

Confusion Matrix

Cross-Validation (5-Fold)

Cross-validation results confirmed good generalization with minimal overfitting.

Visualizations
1️.Ticket Category Distribution

Shows how tickets are distributed across departments.

2️.Confusion Matrix — Category Prediction

Helps identify misclassification patterns between ticket types.

3️.Priority Classification Report Visualization

Shows precision, recall, and F1-score per priority level.

Prediction System

A reusable prediction function was created:

predict_ticket("My account is locked and I need urgent access")

Business Impact

This system can:

Reduce manual ticket sorting workload

Automatically route tickets to the correct department

Detect urgent issues faster

Improve customer support efficiency

Support SLA compliance


Project Structure
FUTURE_ML_02/
│
├── data/
│   └── customer_support_tickets.csv
│
├── task_2.ipynb
│
├── ticket_distribution.png
├── category_cm.png
├── priority_cm.png
│
└── README.md

Conclusion

This project demonstrates the real-world application of:

Natural Language Processing (NLP)

Text Vectorization using TF-IDF

Multi-output Machine Learning Classification

Model Evaluation and Cross-Validation

The developed system successfully predicts both ticket category and priority level, making it highly useful for automated customer support environments.
