# Maersk Supply Risk Analysis

This repository contains a comprehensive analysis and modeling of the Maersk Supply data. The aim is to predict the class of a given instance based on various textual and categorical features, in this case, the cause of a part failure based on the symptoms. We have applied multiple machine learning methods to achieve this, including Random Forest, XGBoost, and MLP (Multi-Layer Perceptron).

## Introduction

In this project, we aim to classify instances of Maersk Supply data into various classes based on textual and categorical features. The dataset includes features such as 'Object', 'Group', 'Object_Type', 'Directive', 'Work_Description', and 'Completion_Note'. We employ several machine learning techniques to build robust models for this classification task.

## Setup

### Prerequisites

- Python 3.x

### Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/SySyAli/nlp_risk_prediction.git
cd nlp_risk_prediction
```
Download the depedencies needed to run the notebooks:
```bash
pip install requirements.txt
```

## Data

The dataset used in this project is obtained from Maersk Supply. The key features and the target variable ('EBS1') are used for analysis and modeling. The data is loaded from Excel files and combined into a single DataFrame.

## Preprocessing

1. **Cleaning**: Handle missing values, remove unwanted characters, and lowercasing text.
2. **Text Processing**: Tokenization, lemmatization, and removal of stop words.
3. **Vectorization**: Convert text data into numerical features using TF-IDF and Count Vectorizer.
4. **Encoding**: Encode categorical labels using LabelEncoder.
5. **Handling Imbalanced Classes**: Address class imbalance using techniques like Random Over Sampling.

## Exploratory Data Analysis (EDA)

Several EDA techniques were applied to understand the distribution of data, identify patterns, and visualize the relationships between features. The key visuals include:
- Class distribution of the target variable.
- PCA plot to visualize the high-dimensional TF-IDF features in 2D space.

## Modeling

Random Forest, XGBoost, and MLP were used to find the best model. Scikit-learn's GridSearchCV and RandomSearchCV were used for hyperparameter tuning. Please see the named files for each model use.
