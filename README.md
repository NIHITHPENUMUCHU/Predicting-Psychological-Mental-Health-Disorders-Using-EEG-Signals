# Predicting Psychological Mental Health Disorders From EEG Signals

This repository contains the implementation of our project, which leverages EEG data and machine learning techniques (Random Forests and Neural Networks) to predict psychological mental health disorders. The project aims to explore the potential of EEG signals in diagnosing and classifying various mental health conditions.


## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
  - [Content](#content)
  - [Acknowledgements](#acknowledgements)
- [Methods Used](#methods-used)
- [Installation](#installation)
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

### Context
A psychiatric disorder is a mental illness diagnosed by a mental health professional that greatly disturbs your thinking, moods, and/or behavior and seriously increases your risk of disability, pain, death, or loss of freedom. In addition, your symptoms must be more severe than expected in response to an upsetting event, such as normal grief after the loss of a loved one.

A large number of psychiatric disorders have been identified. Chances are that, whether or not you or someone close to you has been diagnosed with a psychiatric disorder, you know something about one or more of the following examples:
- Depression
- Personality disorders
- Anxiety disorders
- Schizophrenia
- Eating disorders
- Addictive behaviors

### Content
EEG Dataset with approximately 1,000 attributes for identifying psychiatric disorders.

### Acknowledgements
Park, S. M. (2021, August 16). *EEG machine learning*. Retrieved from [osf.io/8bsvr](https://osf.io/8bsvr)  
Please credit the original author if you want to use this dataset for your research.  
The source of the dataset is available [here](https://osf.io/8bsvr/).

## Methods Used
- **Preprocessing:** EEG signal cleaning, feature extraction, and normalization.
- **Machine Learning Models:**
  - Random Forest Classifier
  - Neural Network Classifier
- **Validation:** Cross-validation techniques to evaluate model performance.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC.

## Installation
To run this project, ensure you have the following installed:
- Python 3.8+
- Libraries: NumPy, Pandas, Matplotlib, Seaborn

## Results
The following are the key results from our models:

### Improved Hybrid Model

#### Main Disorder Classification
- **Accuracy:** 0.4233  
- **Classification Report:**

```plaintext
                                    precision    recall  f1-score   support

                Addictive disorder       0.58      0.62      0.60        34
                  Anxiety disorder       0.00      0.00      0.00        16
                   Healthy control       0.43      0.47      0.45        19
                     Mood disorder       0.38      0.89      0.53        56
     Obsessive compulsive disorder       0.00      0.00      0.00         9
                     Schizophrenia       0.00      0.00      0.00        20
Trauma and stress related disorder       0.00      0.00      0.00        35

                          accuracy                           0.42       189
                         macro avg       0.20      0.28      0.23       189
                      weighted avg       0.26      0.42      0.31       189
```

#### Binary Classification (Healthy vs. Unhealthy)
- **Accuracy:** 0.9101  
- **Classification Report:**

```plaintext
              precision    recall  f1-score   support

   Unhealthy       0.96      0.94      0.95       170
     Healthy       0.54      0.68      0.60        19

    accuracy                           0.91       189
   macro avg       0.75      0.81      0.78       189
weighted avg       0.92      0.91      0.91       189
```

---

### Neural Network

#### Main Disorder Classification
- **Accuracy:** 0.3122  
- **Classification Report:**

```plaintext
                                    precision    recall  f1-score   support

                Addictive disorder       0.35      0.41      0.38        34
                  Anxiety disorder       0.05      0.06      0.06        16
                   Healthy control       0.50      0.47      0.49        19
                     Mood disorder       0.38      0.38      0.38        56
     Obsessive compulsive disorder       0.33      0.33      0.33         9
                     Schizophrenia       0.21      0.20      0.21        20
Trauma and stress related disorder       0.26      0.20      0.23        35

                          accuracy                           0.31       189
                         macro avg       0.30      0.29      0.29       189
                      weighted avg       0.31      0.31      0.31       189
```

#### Binary Classification (Healthy vs. Unhealthy)
- **Accuracy:** 0.9153  
- **Classification Report:**

```plaintext
              precision    recall  f1-score   support

           0       0.94      0.96      0.95       170
           1       0.60      0.47      0.53        19

    accuracy                           0.92       189
   macro avg       0.77      0.72      0.74       189
weighted avg       0.91      0.92      0.91       189
```

---

### Random Forest

#### Main Disorder Classification
- **Accuracy:** 0.4074  
- **Classification Report:**

```plaintext
                                    precision    recall  f1-score   support

                Addictive disorder       0.43      0.68      0.53        34
                  Anxiety disorder       0.00      0.00      0.00        16
                   Healthy control       0.60      0.16      0.25        19
                     Mood disorder       0.41      0.89      0.56        56
     Obsessive compulsive disorder       1.00      0.11      0.20         9
                     Schizophrenia       0.00      0.00      0.00        20
Trauma and stress related disorder       0.00      0.00      0.00        35

                          accuracy                           0.41       189
                         macro avg       0.35      0.26      0.22       189
                      weighted avg       0.31      0.41      0.30       189
```

#### Binary Classification (Healthy vs. Unhealthy)
- **Accuracy:** 0.9048  
- **Classification Report:**

```plaintext
              precision    recall  f1-score   support

           0       0.90      1.00      0.95       170
           1       1.00      0.05      0.10        19

    accuracy                           0.90       189
   macro avg       0.95      0.53      0.52       189
weighted avg       0.91      0.90      0.86       189
```


## Future Work
- Integrating other datasets to improve model robustness.
- Developing a hybrid model for enhanced accuracy.
- Deploying the model as a web application for real-world usage.

## Contributors
- Penumuchu Nihith
- Shaik Mohammed Shoaib

## License
This project is licensed under the [MIT License](LICENSE).








