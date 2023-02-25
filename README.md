# Facial Expression Recognition

## Introduction
This project aims to classify the emotion on a person's face into one of the seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral), using convolutional neural networks. 

## About
It uses fer2013 database which you can download from the link below:

https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data

This project consists of a single notebook which has the following:

* Data pre-processing
* Training model
* Testing model and comparing results

_I have included a pre-trained model to compare my results._

## Process for training
- First, we import the dataset and initialize our **X_train, y_train, X_test, y_test** .

- Then we create our **model architecture**. Following is my model architecture:

![architecture](https://drive.google.com/u/2/uc?id=1HmnQIZUf8jjffmUSm_3DU6QIZl6x3r5F&export=download)

## Process for predicting
- First, we use **haar cascade** to detect faces in the given image and crop the face accordingly.

- Then we reshape our image to **48 * 48** pixels to meet the requirements of our trained model and pass it as an input to our model.

- The output is a list containing seven probabilities, each for an emotion.

- The index of **maximum probability** from the list indicates the emotion (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).

## Final notebook with all code

[Complete Notebook](https://github.com/akash720/Facial-expression-recognition/blob/master/complete_notebook.ipynb)

