# Credit Card Fraud Detection using Supervised Algorithms

This project tackles the issue of detecting fraudulent transactions from a dataset of credit card transactions. The dataset used is highly imbalanced, with only 0.17% of transactions classified as fraud. Multiple supervised learning algorithms were employed to build a reliable fraud detection model.

## Dataset
The dataset is sourced from the [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud). It contains 284,807 transactions, 492 of which are fraudulent. Features are anonymized and scaled due to privacy reasons.

## Project Workflow
1. **Data Exploration & Preprocessing**:
   - Analyzed data distribution of features like transaction amount and time.
   - Identified class imbalance and used Random Under-Sampling to balance the data.
   - Correlation analysis helped in selecting important features.

2. **Modeling**:
   - Algorithms applied: Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), and Decision Tree.
   - **Grid Search** was performed to optimize hyperparameters for each model.

3. **Evaluation**:
   - Cross-validation scores and ROC-AUC scores were used to compare models.
   - **Logistic Regression** emerged as the top model with a cross-validation accuracy of **94.54%** and strong AUC-ROC performance.

4. **Key Results**:
   - **Logistic Regression** showed the best performance in terms of generalizability and stability.
   - **SVC** was a close second, while KNN and Decision Tree showed higher variance and slightly lower scores.

## Visualizations
- Distribution of transaction amounts and correlation heatmaps for feature analysis.
- ROC curves and learning curves for model evaluation.

## Conclusion
Logistic Regression stands out as the most reliable model for detecting fraudulent transactions due to its high accuracy, low variance, and strong ROC-AUC score.

---

### Installation
To run this project, install the required libraries:

```bash
pip install -r requirements.txt
