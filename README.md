# Zidio-Internship---Project-2---Emotion-Recognition-
This project aims to perform emotion recognition from speech using a dataset of emotional speech samples. The goal is to preprocess the audio data, extract features, and train machine learning models to classify the emotions in the speech samples. 


*****Emotion Recognition using LSTM on Toronto Emotional Speech Set (TESS) Dataset*****

Project Overview
This project aims to recognize emotions from speech using a Long Short-Term Memory (LSTM) neural network. We use the Toronto Emotional Speech Set (TESS) dataset, which consists of recordings of actors saying the same set of phrases in different emotional states. The goal is to build and evaluate a model that can accurately classify the emotion conveyed in the speech.

Key Steps and Features of the Project:
***1. Data Loading and Preprocessing***

Import Necessary Libraries: Import essential libraries such as pandas, numpy, librosa, seaborn, matplotlib, and Keras.
Download and Unzip Dataset: Use the Kaggle API to download and unzip the TESS dataset.
Data Collection: Traverse the dataset directory to collect file paths and corresponding labels (emotions).
Create DataFrame: Create a DataFrame to store the file paths and labels.

***2. Exploratory Data Analysis (EDA)***
Label Distribution Visualization: Use count plots to visualize the distribution of different emotion labels in the dataset.
Waveplot and Spectrogram: Define functions to plot the waveform and spectrogram of audio files to understand the differences in audio characteristics for different emotions.

***3. Feature Extraction***
Label Encoding: Encode the categorical emotion labels into numerical format and convert them to categorical format for model training.

***4. Model Training with LSTM***
Data Splitting: Split the data into training and testing sets.
Data Reshaping: Reshape the data to fit the input requirements of the LSTM model.
Build LSTM Model: Define an LSTM model with masking, LSTM, dropout, and dense layers.
Model Compilation: Compile the model using categorical cross-entropy loss and Adam optimizer.
Model Training: Train the model on the training data and validate it on the validation set.

***5. Model Evaluation***
Model Evaluation: Evaluate the model on the test set and print the accuracy.
Training History Visualization: Plot the training and validation accuracy and loss over epochs to analyze the model's performance.

***6.Visualization of Results***
The code evaluates the model's performance on test data and prints the accuracy. It then plots training and validation accuracy as well as loss over epochs. This visual representation helps in understanding the model's performance and how it evolves during training.
