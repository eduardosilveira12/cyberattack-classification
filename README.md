# Cyberattack Classification Using Deep Neural Networks
Overview

This repository contains the implementation of a machine learning project aimed at detecting and classifying cyberattacks in network traffic. Using the UNSW-NB15 dataset and deep neural network architectures, the project tackles two key tasks:

    Binary Classification: Predict whether network traffic is benign or malicious.
    Multiclass Classification: Identify specific types of attacks (e.g., DoS, worms, backdoors).

Key Features

    Implementation of Binary and Multiclass classification models.
    Utilizes the UNSW-NB15 dataset, a modern and comprehensive network intrusion dataset.
    Preprocessing pipeline including normalization, one-hot encoding, and train/test split.
    Support for multiple deep learning architectures:
        Dense Neural Networks (MLP)
        Convolutional Neural Networks (CNN)
        Recurrent Neural Networks (LSTM/GRU)
        Hybrid architectures (CNN + RNN)
    Evaluation metrics focused on real-world relevance: F1-Score, Accuracy, AUROC, and Confusion Matrix.

Dataset

The UNSW-NB15 dataset combines real and simulated network traffic. It includes:

    2.54 million records:
        Normal traffic: 2.2 million samples.
        Attacks: 9 categories such as Fuzzers, DoS, Exploits, and Worms.
    File formats: CSV and Parquet for flexible data handling.