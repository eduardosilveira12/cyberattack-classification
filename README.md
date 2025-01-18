# Cyberattack Classification Using Deep Learning

This project utilizes the **UNSW-NB15 dataset** to develop a deep learning model for multi-class classification of cyberattacks. By leveraging techniques like data preprocessing, feature engineering, and advanced deep learning architectures, the project aims to address challenges in network intrusion detection, including class imbalance and feature selection.

## Table of Contents

1. [Introduction](#introduction)  
2. [Dataset Description](#dataset-description)  
3. [Problem Statement](#problem-statement)  
4. [Data Preprocessing](#data-preprocessing)  
5. [Model Architecture](#model-architecture)  
6. [Training and Evaluation](#training-and-evaluation)  
7. [Results](#results)  
8. [Conclusions](#conclusions)  
9. [References](#references)  

## Introduction

Cybersecurity is critical in today's connected world. This project explores deep learning as a solution for classifying network traffic into normal or attack categories. The goal is to build a robust model capable of real-time intrusion detection.

## Dataset Description

The **UNSW-NB15** dataset comprises normal network traffic and nine types of attacks:
- Fuzzers
- Analysis
- Backdoors
- DoS
- Exploits
- Generic
- Reconnaissance
- Shellcode
- Worms

The dataset contains 49 features, including network metrics and categorical attributes.

## Problem Statement

The project aims to:
- Develop a multi-class classification model for network traffic.
- Handle significant class imbalance in cybersecurity datasets.
- Create a robust preprocessing pipeline for network traffic data.

## Data Preprocessing

Data preprocessing includes:
- **Feature Engineering**: Creating new features like `bytes_per_packet`, `packets_per_second`, and statistical metrics.  
- **Outlier Handling**: Using methods like the Interquartile Range (IQR).  
- **Class Balancing**: Addressing imbalance with techniques like Tomek Links and ADASYN.  
- **Scaling and Encoding**: RobustScaler for numerical features and LabelEncoder for categorical features.

## Model Architecture

The optimized GRU-based architecture includes:
- Bidirectional GRU layers to capture temporal dependencies.
- Regularization (L1 and L2) to prevent overfitting.
- Dropout layers for enhanced generalization.
- A dense output layer with softmax activation for multi-class classification.

## Training and Evaluation

The model is trained with:
- **Optimizer**: Adam (learning rate: 0.0003884).  
- **Loss Function**: Sparse categorical crossentropy.  
- **Metrics**: Accuracy, precision, recall, and F1-score.  
- **Callbacks**: Early stopping, learning rate reduction, and model checkpointing.  

## Results

The trained model achieved:
- **Accuracy**: [Insert Value]  
- **Precision**: [Insert Value]  
- **Recall**: [Insert Value]  
- **F1-Score**: [Insert Value]  

Confusion matrices and classification reports provide insights into performance per class.

## Conclusions

This project demonstrated the effectiveness of deep learning in classifying network attacks. Future directions include:
- Evaluating on other datasets.
- Exploring real-time deployment.
- Investigating other machine learning algorithms.

## References

- UNSW-NB15 Dataset: [UNSW Canberra Cybersecurity](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/)  (original)
- UNSW-NB15 Dataset: [Kaggle] (https://www.kaggle.com/datasets/dhoogla/unswnb15/data) (This is the version I have used in my implementation.)
- Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press.
