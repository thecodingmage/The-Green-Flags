# The-Green-Flags
AI Content Moderation System

About the Project:
We are currently running this model locally for development and testing purposes. However, we're actively working on deploying it to a website, making it accessible to everyone very soon. Stay tuned for updates!

Introduction:
This project implements an automated content moderation system that classifies textual content as appropriate or inappropriate for public display. Leveraging machine learning models (LSTM and BERT) and natural language processing techniques, the system analyzes textual data in real-time to provide classification results. Additionally, the project extends its functionality to extract text from images and memes (using Google Cloud Vision API ), enabling classification based on the extracted textual content.

Files Included:
Data_Preprocessing.ipynb: Jupyter notebook for loading and preprocessing the dataset (hate_offensive_data.csv) to create a new CSV file (preprocessed_data.csv).
LSTM.ipynb: Jupyter notebook for training and evaluating the LSTM model for text classification using the preprocessed data.
BERT.ipynb: Jupyter notebook for training and evaluating the BERT model for text classification using the preprocessed data.
requirements.txt: File listing the Python libraries required to be installed before executing the code.
Flask_app/main.py: Python file for the Flask application. This file handles text and image inputs through a web browser, loads the trained BERT model, and accesses the Google Cloud Vision API for text extraction from images.
Flask_app/templates/index5.html: HTML page for the Flask application.
Flask_app/app.yaml: Configuration file required for deploying the Flask application on Google App Engine.

Results
To assess the performance of our classification models, we conducted a comprehensive evaluation using key metrics such as accuracy, precision, recall, and the F1 score. These metrics provide valuable insights into the abilities of classifiers to accurately categorize textual content as either inappropriate or appropriate for public display.

Metric	LSTM	BERT

Accuracy	93.65%	95.62%

Precision	95.97%	97.20%

Recall	96.41%	97.55%

F1 Score	96.19%	97.37%

Through these evaluations, BERT demonstrated superior performance over LSTM, particularly in terms of accuracy, precision, recall, and F1 score. BERT's enhanced capabilities make it the preferred choice for accurate and reliable content moderation tasks.
