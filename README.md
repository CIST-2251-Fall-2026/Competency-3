# Dry Bean Model Comparison
Project Purpose
This project compares machine learning models for predicting dry bean varieties from image-based measurements. The goal is to compare accuracy, speed, overfitting, interpretability, and maintainability.
Models
The models tested were Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting.
I used an 80/20 stratified train/test split and 5-fold stratified cross-validation.
Results
All four models reached around 90–93% accuracy. Gradient Boosting had the highest overall accuracy, while Logistic Regression provided a strong balance of accuracy, speed, simplicity, and interpretability.
Random Forest reached 100% training accuracy but about 92% test accuracy, showing evidence of overfitting.
Clustering
I used K-Means with seven clusters without providing the Class labels. The Adjusted Rand Score was about 0.67 and the Silhouette Score was about 0.31. Some varieties formed clearer natural groups than others.
Recommendation
I would consider Logistic Regression for the first production prototype because it provides good accuracy while remaining fast, simple, explainable, and easy to maintain.
Gradient Boosting would also be worth further testing because it achieved slightly higher accuracy.
More real-world testing would be needed before using either model to control production sorting equipment.
Setup
Install the required packages:
pip install -r requirements.txt
Open dry_bean_model_comparison.ipynb and run all cells in order.
Dataset
Koklu, M., and Ozkan, I. A. (2020). Dry Bean [Dataset]. UCI Machine Learning Repository.
DOI: https://doi.org/10.24432/C50S4B
License: CC BY 4.0
Reproducibility
The project uses random_state=42 where applicable so the results can be reproduced. The repository includes the notebook, dataset, requirements file, results, and documentation.
AI Use
I used ChatGPT to help understand the assignment, organize the notebook, troubleshoot errors, and explain parts of the code. I verified the results by running the notebook and reviewing the outputs.