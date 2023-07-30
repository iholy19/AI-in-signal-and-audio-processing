# Dataset
https://www.kaggle.com/competitions/tensorflow-speech-recognition-challenge/data
5 classes are chosen to classify: yes, no, wow, left, right

# Objective
To classify the audio commands

# Code Development
- Extract features from audio using librosa and store them as dataframe
- Convert audio into spectrogram images
- Train the model with
  * SVM - Polynomial and SVM kernel
  * BPNN
  * CNN - VGG16
 
CNN with spectrogram is the best model for classifying this audio as images. The accuracy achieved is greater than 85%
