# Plagiarism Project, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

This project builds a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.

**Notebook 2: Feature Engineering**
* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy the Model in SageMaker**
* Upload the train/test feature data to S3.
* Define a binary classification model and a training script.
* Train the model and deploy it using SageMaker.
* Evaluate the deployed classifier.

- - - -

> Please note this is a project from the Udacity Machine Learning Engineering Nanodegree Program. Some of the code templates were provided by Udacity, and I provided my codes to complete the project. Some people put the whole project on their Github repos without giving any credit to Udacity. This is not the right thing to do. As professional developers, we should give credit where credit's due. I hope this repo will help other students with their learning journey.