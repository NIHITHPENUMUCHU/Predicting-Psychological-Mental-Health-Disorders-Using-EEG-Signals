# Predicting Psychological Mental Health Disorders Using EEG Signals

This repository contains the implementation of our project, which leverages EEG data and machine learning techniques (Random Forests and Neural Networks) to predict psychological mental health disorders. The project aims to explore the potential of EEG signals in diagnosing and classifying various mental health conditions.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Methods Used](#methods-used)
- [Results](#results)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Overview
Mental health disorders are a growing concern worldwide, and early detection is crucial for effective treatment. This project uses machine learning models to analyze EEG signals and predict mental health disorders, providing an automated, non-invasive diagnostic approach.

Key Objectives:
- To utilize EEG signals for mental health disorder prediction.
- To compare the performance of Random Forests and Neural Networks.
- To analyze the significance of EEG features in classification.

## Dataset
We used the **Auditory Evoked Potential EEG-Biometric dataset**, which includes:
- EEG recordings from multiple subjects.
- Both background and task-related data.
- Groups classified by mental arithmetic performance.

The dataset was processed and augmented to ensure robust model performance.

## Methods Used
- **Preprocessing:** EEG signal cleaning, feature extraction, and normalization.
- **Machine Learning Models:**
  - Random Forest Classifier
  - Neural Network Classifier
- **Validation:** Cross-validation techniques to evaluate model performance.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC.

## Results
The following are the key results from our models:
- **Random Forest:**
  - Accuracy: XX%
  - F1-Score: XX%
- **Neural Network:**
  - Accuracy: XX%
  - F1-Score: XX%

The Neural Network model demonstrated slightly better performance in predicting disorders.

## Future Work
- Integrating other datasets to improve model robustness.
- Developing a hybrid model for enhanced accuracy.
- Deploying the model as a web application for real-world usage.

## Contributors
- Penumuchu Nihith
- Shaik Mohammed Shoaib

## License
This project is licensed under the [MIT License](LICENSE).
