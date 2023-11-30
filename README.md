# Sign Language Detector using MediaPipe and LSTM Neural Network
This repository contains code for a sign language detection system utilizing the MediaPipe library for pose and hand tracking, combined with a Long Short-Term Memory (LSTM) Neural Network for classification.

## Overview
The project includes:

- code.ipynb: Jupyter Notebook containing the code for data collection, preprocessing, model training, and live testing of the sign language detector.
- action.h5: Saved model file after training the LSTM Neural Network.
- MP_data: Directory to store collected keypoints data for training and testing.
- Logs: Folder for TensorBoard logs to monitor neural network progress.

## Setup and Requirements
### Installation
1. Clone this repository:
   ```
   git clone https://github.com/Devansh-Gupta-Official/sign-language-detector.git
   cd sign-language-detector
   ```
2. Install the required libraries:
   ```
   pip install -r requirements.txt
   ```
### Usage
- Open the Jupyter Notebook code.ipynb to run the code.
- Ensure a webcam is connected for live sign language detection.
- Adjust parameters such as no_sequences, sequence_length, etc., for data collection as needed.

## Data Collection and Training
1. The notebook contains code for capturing webcam frames, extracting keypoints using MediaPipe, and storing the data in the MP_data directory.
2. The data is preprocessed, split into training and testing sets, and used to train the LSTM Neural Network for sign language classification.

## Model Evaluation
Evaluation metrics such as multilabel confusion matrix and accuracy score are calculated on the trained model using the testing set.

## Live Sign Language Detection
- The notebook provides a live demonstration of sign language detection using the trained model.
- OpenCV displays the webcam feed, tracks pose and hand landmarks, predicts signs, and visualizes the detected signs with real-time feedback.

## Results
![image](https://github.com/Devansh-Gupta-Official/sign-language-detector/assets/100591612/c214ec7f-fa04-4025-90fc-5f07fb7212e0)
![image](https://github.com/Devansh-Gupta-Official/sign-language-detector/assets/100591612/fb94b619-de13-4d05-9de9-2f3ada9d0856)
![image](https://github.com/Devansh-Gupta-Official/sign-language-detector/assets/100591612/0b4e21b4-00f8-4284-814b-594429d1b488)

