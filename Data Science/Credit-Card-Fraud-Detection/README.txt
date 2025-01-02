
# Credit Card Fraud Detection

This repository contains a machine learning pipeline for detecting fraudulent credit card transactions using various classification models. The dataset used for training and testing is sourced from [Kaggle's Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Models Evaluated](#models-evaluated)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Credit card fraud is a significant concern in the financial industry. This project uses machine learning algorithms to classify transactions as fraudulent or non-fraudulent. The dataset is highly imbalanced, and various techniques and metrics are utilized to address this challenge.

## Features
- Implements multiple machine learning models from `sklearn`, `xgboost`, `lightgbm`, and `catboost`.
- Evaluates models using accuracy, cross-validation scores, and other metrics.
- Handles imbalanced datasets using appropriate techniques.
- Scalable pipeline for feature scaling and model evaluation.

## Dataset
The dataset contains 284,807 transactions with 31 features:
- **Time**: Time elapsed between the transaction and the first transaction.
- **V1 to V28**: PCA-transformed features.
- **Amount**: Transaction amount.
- **Class**: Target variable (0 for non-fraudulent, 1 for fraudulent).

### Dataset Link
[Download the dataset from Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd credit-card-fraud-detection
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Place the dataset (`creditcard.csv`) in the appropriate directory.
2. Run the main script to train and evaluate models:
   ```bash
   python main.py
   ```

## Models Evaluated
The following models were tested for this project:
- Logistic Regression
- Ridge Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost
- LightGBM
- CatBoost
- Support Vector Machines
- Naive Bayes
- Neural Networks (MLPClassifier)
- Isolation Forest (anomaly detection)

### Performance Metrics
Each model is evaluated using:
- **Accuracy**
- **Cross-Validation Score**
- **ROC-AUC**

## Results
Some of the best-performing models include:
- **Random Forest Classifier**: Accuracy: 99.96%, Cross-Validation Score: 99.95%
- **CatBoost Classifier**: Accuracy: 99.96%, Cross-Validation Score: 99.96%
- **XGBoost**: Accuracy: 99.96%, Cross-Validation Score: 99.96%

### Limitations
- Models like `MultinomialNB` and `CategoricalNB` failed due to the presence of negative values in the dataset.
- Memory-intensive models like `GaussianProcessClassifier` encountered limitations due to dataset size.

## Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
