📌 Speech Classification Project (Male vs Female)

Brief Description:
This project classifies speech audio clips into Male and Female categories using audio feature extraction and machine learning models, including a Naïve Bayes classifier from scratch and Bagging ensembles.

🚀 Overview

The goal of this project is to analyze audio recordings and predict the speaker's gender based on extracted audio features such as MFCCs, spectral features, zero-crossing rate, and RMS.

Target Classes:

0 → Male

1 → Female
🧠 Problem Statement

Gender recognition from speech is useful in voice assistants, call centers, and audio analytics.

Audio data is complex, requiring careful preprocessing and feature extraction for accurate classification.

Simple models like Naïve Bayes may underperform on raw features, motivating the use of ensemble methods.

💡 Solution

Step 1: Extract features from audio files:

MFCCs (13 coefficients)

Spectral Centroid

Spectral Rolloff

Zero Crossing Rate

RMS Energy

Step 2: Build classifiers:

Naïve Bayes (from scratch)

Logistic Regression

Step 3: Improve performance using Bagging ensembles.

🏗️ System Architecture
Input: .wav audio files
↓
Preprocessing: median filtering, silence removal, normalization
↓
Feature Extraction: MFCCs, spectral centroid, spectral rolloff, zero-crossing rate, RMS
↓
Train/Test Split (70/30)
↓
Machine Learning Models:
    - Naïve Bayes (from scratch)
    - Logistic Regression
    - Bagging Ensemble (Naïve Bayes / Logistic Regression)
↓
Output: Predicted Gender (Male/Female)

🛠️ Technologies Used

Python

Libraries: librosa, pydub, numpy, pandas, scipy, scikit-learn, matplotlib, seaborn

Audio preprocessing and feature extraction

📊 Models / Algorithms

Naïve Bayes From Scratch

Calculates class-wise mean and variance for features

Likelihood modeled as Gaussian

Posterior probability via Bayes theorem

Accuracy: ~85.8%

Bagging Ensemble

Bootstrap sampling with multiple base models

Base models: Naïve Bayes or Logistic Regression

Predictions aggregated via majority voting

Accuracy:

Naïve Bayes Bagging: 88.3%

Logistic Regression Bagging: 93.3%

Evaluation Metrics:

Accuracy

Precision

Recall

F1 Score

🧪 Results

Naïve Bayes From Scratch:

Accuracy: 85.8%

Precision: 81.8%

Recall: 91.5%

F1 Score: 86.4%

Bagging Naïve Bayes:

Accuracy: 88.3%

Precision: 84.6%

Recall: 93.2%

F1 Score: 88.7%

Bagging Logistic Regression:

Accuracy: 93.3%

Precision: 89.2%

Recall: 98.3%

F1 Score: 93.5%

Use Cases

Gender detection for voice assistants

Call center analytics

Audio-based biometric authentication

📄 License

This project is for educational purposes.
