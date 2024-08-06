# Advanced Fraud Detection System

This project implements an Advanced Fraud Detection System using a credit card transaction dataset. The system leverages machine learning techniques to effectively identify and predict fraudulent transactions, aiming to enhance the accuracy of fraud detection and minimize financial losses.

## Project Overview

Fraud detection is critical in the financial sector to prevent unauthorized transactions and reduce financial losses. This project explores various machine learning models to detect fraudulent transactions in a credit card dataset provided by Kaggle.

### Dataset

The dataset used in this project is the "Credit Card Transactions Dataset" available on [Kaggle](https://www.kaggle.com/datasets/priyamchoksi/credit-card-transactions-dataset). It includes features such as transaction amount, merchant category, and transaction time, essential for identifying fraudulent activities.

## Methodology

### Data Preprocessing

- **Handling Missing Values**: Missing data was identified and imputed where appropriate to ensure the dataset's completeness.
- **Feature Encoding**: Categorical features such as merchant categories and transaction types were encoded to numerical values using techniques like label encoding, facilitating model training.
- **Feature Engineering**: Additional features were derived, such as extracting the transaction hour from timestamps, to capture temporal patterns in fraud occurrence.

### Model Building

Multiple machine learning algorithms were employed to build predictive models, including:

1. **Logistic Regression**: Used as a baseline model due to its simplicity and interpretability.
2. **Decision Tree**: Provides a tree-based structure to capture non-linear patterns in data.
3. **Random Forest**: Utilizes ensemble learning to improve prediction accuracy and robustness.
4. **Gradient Boosting**: Sequentially builds models that reduce errors from previous models.
5. **Neural Networks**: Employs deep learning to model complex relationships within the dataset.

### Model Evaluation

- **Metrics**: Models were evaluated using metrics such as precision, recall, F1-score, and ROC-AUC. These metrics provide a comprehensive view of each model's performance, particularly in handling the imbalanced nature of fraud detection.

## Results

- **Logistic Regression** showed limitations in detecting fraud, with low recall for fraudulent transactions.
- **Decision Tree** provided better recall and precision but was prone to overfitting.
- **Random Forest** achieved the highest performance, with a high ROC-AUC score, indicating strong discriminative ability.
- **Gradient Boosting** offered good performance with reduced variance compared to Decision Trees.
- **Neural Networks** demonstrated competitive performance, capturing complex patterns effectively.

### Conclusion

The Random Forest model emerged as the most effective for this dataset, offering a balanced trade-off between precision and recall while maintaining a high ROC-AUC score. The project demonstrates the importance of using ensemble methods for fraud detection, highlighting their ability to capture intricate data patterns and mitigate overfitting.

## Future Work

- **Hyperparameter Tuning**: Further optimization of model parameters to enhance performance.
- **Real-Time Implementation**: Integrating the model into a real-time transaction processing system for immediate fraud detection.
- **Explainability**: Using techniques like SHAP (SHapley Additive exPlanations) to provide insights into model decisions and increase transparency.

## Getting Started

### Prerequisites

Ensure you have the following libraries installed:
- NumPy
- Pandas
- Scikit-Learn
- Matplotlib
- Seaborn

### Installation

Clone this repository and install the dependencies:

```bash
git clone https://github.com/Peekaboo64534/Advanced-credit-Fraud-Detection-System.git
pip install -r requirements.txt
