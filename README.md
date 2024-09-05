Amazon Review Score Prediction

Description:
This project predicts the score levels (low, medium, high) of Amazon reviews using metadata and review text. The dataset, sourced from Kaggle, contains over 500,000 reviews for training and 5,000 reviews for testing. The project leverages machine learning to classify reviews into score levels, achieving an accuracy of 84%.

Table of Contents
Overview
Dataset
Installation
Usage
Model Performance
Contributing
License

Overview
The goal of this project is to predict the score_level of Amazon reviews (low, medium, or high). Using various data preprocessing techniques and machine learning algorithms, the model was trained to predict the score level based on the review's metadata and text. The project achieved 84% accuracy on the test dataset.

Dataset
The dataset is sourced from Kaggle and consists of the following files:

foods_training.csv: Contains 518,358 reviews with associated score_level for training.
foods_testing.csv: Contains 5,000 reviews for testing without score_level. The task is to predict these values.
sample_submission.csv: A template for Kaggle submission.

The fields in the dataset include:
ID - Unique identifier for the review.
productID - Unique identifier for the product.
userId - Unique identifier for the user.
helpfulness - Helpfulness rating for the review.
summary - Summary of the review.
text - Full review text.
score_level - Low, medium, high (prediction goal).

Installation

Install the required dependencies:
pip install -r requirements.txt

Usage

Prepare the dataset:
Download the dataset from Kaggle.
Place the CSV files in the data/ folder.

Run the model:
python train_model.py

Make predictions on the test dataset:
python predict.py --input data/foods_testing.csv --output submission.csv

Submit the submission.csv file to Kaggle for evaluation.

Model Performance
The final model achieved an accuracy of 84% in predicting the score_level on the testing dataset.

