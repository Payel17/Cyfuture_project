# Cyfuture_project
AI-ML Project
# Introduction
Emotion detection in text data involves identifying the emotions expressed in textual data. This can be a challenging task since emotions are often expressed in complex and subtle ways. 
This project focuses on building a machine learning-based emotion detection system that classifies text into emotional categories such as joy, anger, sadness, fear, and more. Using natural language processing (NLP) techniques and popular ML algorithms like Logistic Regression, Random Forest, and Support Vector Machines, the model learns to understand and predict the underlying emotions in a given text input.
# Dataset
Two datasets used for this project contains text data labeled with one of six emotions: anger, fear, joy, love, sadness,and surprise.One for taining purpose and another for testing purpose.The training dataset contains a total of 15982 rows and testing dataset contains a total of 1975 rows.

Annotations of different emotions:
Anger    0
Fear     1
Joy      2
Love     3
Sadness  4
Surprise 5
# Methodology
This project follows a supervised machine learning approach for detecting emotions from text data. The methodology is divided into several stages:
1.Data Collection: Two datasets are used: training.csv and test.csv.Each record consists of a text field (user-generated text) and a corresponding label (emotion class).

2.Data Preprocessing: Combined both training and test datasets into one for unified preprocessing.Applied text cleaning using the NeatText library:Removed Punctuation,Removed stopwords. Created a new column clean_text containing the cleaned version of the input.

3.Feature Extraction: Here Used TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to convert text into numerical features.Considered unigrams and bigrams (ngram_range=(1,2)) to better capture context and local phrase patterns.

4.Model Training: The cleaned data was split into training (80%) and testing (20%) sets using train_test_split from Scikit-learn.The model used for this project is a Logistic Regression ,Support Vector Machine,Random Forest Classifier.

5.Model evaluation: The trained model is evaluated on the test data to measure its accuracy,confusion matrix and classification report in detecting emotions in text data.
# Results
The Logistic Regression achieved an accuracy of 87.22% on the data.
The Support Vector Machine achieved an accuracy of 88.30% on the data.
The Random Forest Classifier achieved an accuracy of 88.27% on the data.



