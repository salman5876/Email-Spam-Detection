# Email Spam Detection Project

This project focuses on building a machine learning model to detect spam emails. It involves preprocessing the data, training multiple models, and evaluating their performance. The primary goal is to develop a reliable classifier that can accurately identify whether an email is spam or not.

## Dataset
in dataset gathering process i checked many of datasets related to spam email (from kaggle github etc..)
from all of them i choose those two dataset but datasets are imbalance so i blanced both dataset first by reducing some rows
(to minimize the impact of reduction to dataset i integrate two same type dataset)
It contains labeled emails, where each email is classified as either spam (1) or not spam (0). 
The dataset includes features such as the subject line and the email content.

## Preprocessing
The preprocessing steps include:
- Removing unnecessary columns like 'Unnamed: 0' and 'label_num'.
- Removing features like 'label' and 'Unnamed'.
- Tokenizing the text data.
- Vectorizing the text data using techniques like CountVectorizer or TF-IDF.
- Splitting the dataset into training and testing sets.

## Models Trained
Three models were trained for this project:
1. Multinomial Naive Bayes
2. LSTM Neural Network

## Model Evaluation
Each model's performance was evaluated using accuracy score.

## Results
The results of each model are as follows:
- Multinomial Naive Bayes: Accuracy = [0.9779151943462897]
- LSTM Neural Network: Accuracy = [0.8763251304626465]

## Usage
To use the trained models for predicting whether an email is spam or not, follow these steps:
1. Load the desired model (e.g., Multinomial Naive Bayes).
2. Vectorize the new email data using the same techniques applied during preprocessing.
3. Use the model's `predict` function to obtain predictions for the new data.

## Files Included
- `spam_email_intern_project.ipynb`: Jupyter Notebook containing preprocessing & model training code.
- `nb_model.pkl`: Pickled file containing the trained Multinomial Naive Bayes model.
- `spam_email_model.pkl`: Pickled file containing the trained LSTM Neural Network model.
- `README.md`: This README file.

## Requirements
- Python 3.x
- Required libraries: pandas, numpy, scikit-learn, keras (for LSTM), pickle
