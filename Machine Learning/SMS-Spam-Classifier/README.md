
# 📩 SMS Spam Classifier

## 📝 Overview
This project is a machine learning-based SMS spam classifier. It processes SMS data to identify messages as either **spam** 🛑 or **ham** ✅. The Jupyter Notebook provided (`SMS-Spam-Classifier.ipynb`) implements a complete pipeline from data preprocessing to model evaluation.

## ✨ Features
- 📂 Data loading and preprocessing
- 🔍 Handling missing values and duplicates
- 📊 Data visualization for class distribution
- 🛠️ Feature engineering using text processing
- 🤖 Model training using machine learning algorithms
- 📈 Evaluation metrics for performance analysis

## 💻 Requirements
The following Python libraries are required to run this notebook:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `nltk`

Ensure you have Python 3.7 or later installed.

## 📁 File Structure
- `spam.csv`: Dataset used for training and evaluation.
- `SMS-Spam-Classifier.ipynb`: Main notebook containing the implementation.

## 🔧 Implementation Steps
1. **Data Loading** 🗂️  
   Load the dataset (`spam.csv`) using `pandas` with appropriate encoding.  
   Columns with unnecessary or null values are removed.

2. **Data Cleaning** 🧹  
   - Drop duplicate rows.  
   - Process text data, including tokenization and removal of special characters.

3. **Exploratory Data Analysis** 📊  
   - Visualize the distribution of spam and ham messages.

4. **Label Encoding** 🔢  
   - Encode the target column to numerical values (0 for ham, 1 for spam).

5. **Feature Extraction** 🧩  
   - Extract text features using `CountVectorizer` or `TF-IDF Vectorizer`.

6. **Model Training** 🏋️‍♂️  
   - Train a machine learning classifier (e.g., Naive Bayes, Logistic Regression).  
   - Perform train-test split for evaluation.

7. **Model Evaluation** 🧪  
   - Calculate metrics like accuracy, precision, recall, and F1-score.

8. **Visualization** 🖼️  
   - Display results and confusion matrix for better interpretation.

## 🚀 How to Run
1. Install the required libraries:
   ```
   pip install numpy pandas scikit-learn matplotlib seaborn nltk
   ```
2. Open the `SMS-Spam-Classifier.ipynb` notebook in Jupyter Notebook or Jupyter Lab.
3. Follow the code cells in sequential order.
4. Place the dataset (`spam.csv`) in the same directory as the notebook.

## 📊 Output
- Classification of SMS messages as spam or ham.
- Model evaluation metrics.
- Plots and visualizations showing data distribution and classifier performance.

## 🔖 Notes
- Ensure the dataset file is properly formatted and placed in the correct directory.
- Feel free to experiment with the model or preprocessing steps to improve performance.

## 👨‍💻 Author
This notebook is designed for educational purposes, demonstrating basic text classification techniques using Python and machine learning libraries.
