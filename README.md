# Sentiment-Analysis
This repository contains the Sentiment Analysis project performed using Databricks and Spark ML. It includes code, datasets, and project documentation.


## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Setup and Installation](#setup-and-installation)
4. [Project Workflow](#project-workflow)
    - [1. Data Preprocessing](#1-data-preprocessing)
    - [2. Model Training](#2-model-training)
    - [3. Evaluation](#3-evaluation)
    - [4. Deployment](#4-deployment)
5. [Key Results](#key-results)
6. [Future Work](#future-work)
7. [License](#license)

---

## Project Overview
This project analyzes a dataset of 100,000+ tweets about ChatGPT to classify public sentiment into three categories:
- **Positive**
- **Neutral**
- **Negative**

The analysis involves:
- Preprocessing text data.
- Using machine learning models for classification.
- Deploying predictions and visualizing trends in sentiment over time.

---

## Technologies Used
- **Programming Languages**: Python, SQL
- **Libraries/Frameworks**: Spark ML, Pandas, Matplotlib, Seaborn
- **Tools**: Databricks, AWS S3, AWS QuickSight
- **Machine Learning Techniques**:
    - Logistic Regression
    - Random Forest
    - Gradient Boosted Trees
    - TF-IDF for text vectorization
    - SMOTE for handling class imbalance

---

## Setup and Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/YourUsername/Sentiment-Analysis.git
    cd Sentiment-Analysis
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Upload the dataset to your Databricks workspace or local environment.
4. Open and run the Jupyter notebooks in the `notebooks/` directory.

---

## Project Workflow

### **1. Data Preprocessing**
- Removed stopwords, URLs, special characters, and emojis from text data.
- Tokenized text and applied TF-IDF for feature engineering.
- Handled class imbalance using SMOTE.

### **2. Model Training**
- Trained the following models:
    - Logistic Regression
    - Random Forest
    - Gradient Boosted Trees
- Used Spark ML pipelines to automate the machine learning workflow.

### **3. Evaluation**
- Evaluated models using:
    - **F1-Score**
    - **ROC-AUC**
    - Confusion Matrix
- Selected the Logistic Regression model for deployment based on its performance.

### **4. Deployment**
- Saved predictions to AWS S3 for further analysis.
- Created Athena tables for querying results.
- Visualized sentiment trends in AWS QuickSight.

---

## Key Results
- Achieved an F1-Score of **0.85** for the Logistic Regression model.
- Visualized sentiment trends, showing positive sentiment growth over time.
- Generated word clouds for each sentiment category to identify key terms.

---

## Future Work
- Expand the dataset with additional social media platforms for broader sentiment coverage.
- Experiment with deep learning models like LSTMs or Transformers for improved accuracy.
- Automate the deployment process using AWS Lambda.


