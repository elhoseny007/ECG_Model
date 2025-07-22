# ECG Arrhythmia Classification using Deep Learning

This project applies deep learning techniques to classify ECG signals using the PTB-XL and MIT-BIH datasets. The model is built using CNN and RNN (GRU) layers and trained on preprocessed ECG signals.

## Project Overview

Electrocardiogram (ECG) classification helps detect heart arrhythmias early. This project uses a hybrid deep learning model (CNN + GRU) to classify ECG signals into five categories based on extracted features.

## Dataset

Two well-known ECG datasets were used:

- **PTB-XL**: A large clinical ECG dataset from PhysioNet.
- **MIT-BIH Arrhythmia Database**: A benchmark dataset for arrhythmia classification.

## 📊 Classes

The model classifies ECG signals into the following 5 categories:
1. Normal
2. Left bundle branch block (LBBB)
3. Right bundle branch block (RBBB)
4. Premature ventricular contraction (PVC)
5. Atrial premature beat (APB)

## 🧪 Model Architecture

- **1D Convolutional Layers**: For feature extraction from time-series signals.
- **MaxPooling Layers**
- **Bidirectional GRU Layers**: For capturing temporal dependencies.
- **Dense + Softmax Output**: For classification into 5 categories.

## 🧼 Preprocessing

- Resampled signals to fixed length (e.g. 500 samples).
- Normalized signal amplitude.
- One-hot encoding of labels.

## ⚙️ Requirements

os
tensorflow
keras
numpy
pandas
matplotlib
scikit-learn
pywt
SMOTE
