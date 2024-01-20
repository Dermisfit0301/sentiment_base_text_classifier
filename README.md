# Hearreview_MVP_sentiment_base_text_classifier
Words from the writer: This repository contains the soul of Hearreview which is classifying statements based on the sentiments they contain. It is the first step in building hearreview and the other steps that including a text summarizer and the dashboard with analytics will be built later as it is outside the scope of the project. The basic prototype is here in this repository which classifies the sentiments using NLP techniques and a classifier. 
This repository has the dataset, the code files, and the pdf files that explain the product. 


Sentiment Analysis Project Documentation
Project Overview
This project is focused on sentiment analysis using machine learning and natural language processing techniques. The goal is to classify text snippets into one of three sentiment categories: positive, neutral, or negative. This documentation provides an overview of the project, the training process, model selection, and the development of a Flask web application.

Dataset and Preprocessing
The project began with a sizable text dataset that included a wide range of product reviews. The dataset was preprocessed to prepare it for machine learning, which included the following steps:

Tokenization: The text data was split into individual words or tokens.
Stemming: To reduce the data's dimensionality and improve processing speed, stemming was applied to the tokens, reducing them to their root forms.
TF-IDF Vectorization: The TF-IDF (Term Frequency-Inverse Document Frequency) vectorization technique was used to convert the text data into numerical format, making it suitable for machine learning models.
Model Training
The sentiment analysis task was approached using various machine learning models. The following are the key phases in the project's evolution:

Conventional ML Models: The initial models consisted of traditional machine learning algorithms like Logistic Regression, Naive Bayes, and Decision Trees. These models provided a baseline accuracy of around 70%.

Artificial Neural Networks (ANN): A more sophisticated approach was implemented using neural networks. After training, the ANN achieved a significant accuracy improvement, reaching around 80%. However, training ANNs can be computationally intensive and time-consuming.

Ensemble Learning Models: In an attempt to further improve accuracy, ensemble learning models such as XGBoost and Random Forest were explored. Among these, Random Forest showed a slight increase in accuracy, reaching approximately 81%.

Hyperparameter Tuning: To optimize the model's performance, hyperparameter tuning was performed on the Random Forest model. However, this step did not result in a significant improvement.

Final Model Selection: In the end, the Random Forest model with the initial hyperparameters was chosen as the final model due to its higher accuracy.

Web Application Development
In order to provide a user-friendly interface for sentiment analysis, a web application was developed. This application allows users to input text snippets and receive predictions regarding their sentiment. The development process included:

Model Export: The trained Random Forest model was saved using the Pickle library to make it available for integration within the web application.

Flask Framework: The web application was built using the Flask web framework, a lightweight yet powerful tool for developing web applications in Python.

HTML : Basic HTML is used to create a simple user interface for entering text snippets.

Backend Integration: The Flask application integrates the saved Random Forest model for sentiment prediction.

