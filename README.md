# SignLanguageNet

This repo contains the code for my Honours (postgraduate) project in which I attempt to harness the power of machine learning to perform sign-language recognition. The proposed solution differs from existing solutions at the time since my solution obviates the need for specialized equipment (such as depth cameras) and instead solely relies on input from a standard computer webcam. The objective of this project was to reconcile the communication barrier experienced by people with hearing impairments by developing a novel solution that can easily be deployed to a mobile phone to perform sign langauge recognition on the go.

## Data

Please download the required dataset [here](https://www.kaggle.com/datamunge/sign-language-mnist).
This dataset contains more than 27,000 training samples of images of American sign language gestures. The each row represents 1 sample in which the grayscale pixel values of a 28x28 hand gesture image are recorded.
The below figure visualizes a few training samples.
<p align="center">
  <img src="https://user-images.githubusercontent.com/26574827/135073319-764e9105-f0ed-4b51-9133-03897f908c53.png"/>
</p>

## Solution

The proposed solution employs a Convolutional Neural Network (CNN) that accepts grayscale images are input and classifies the image as one of the sign language alphabets.
The network contains 5 convolutional layers, each followed by ReLU and downsamples using maxpooling. For regularization purposes, dropout (0.25) is performed.
THe Adam optimizer was used with learning rate = 0.0001.
This solution was developed using Keras.

## Results

Additional results and a comprehensive explanation of the proposed solution is presented in the report (included in this repo).

Below, we present the confusion matrix to illustrate the promise of the proposed solution, despite its simplicity.
<p align="center">
  <img src="https://user-images.githubusercontent.com/26574827/135072899-28832fab-cf9f-49db-82cf-f8a88425e218.png" height="600px"/>
</p>

## Execution

Please refer to the python (Jupyter) notebook which contains all instructions on how the solution should be executed.<br>
Additionally, a demo video is provided that indicates how to execute the solution, presents a demo of the model's performance, and presents a discussion of the project in general.
