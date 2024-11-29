#Harmful Brain Activity Classification Using Machine Learning
Project Overview
This project focuses on the automated classification of harmful brain activity patterns using EEG signals and machine learning models. The goal is to assist in neurocritical care by speeding up the diagnosis of conditions like seizures, GPD, and other abnormal patterns, which traditionally rely on manual and time-intensive interpretation of EEG data.

Motivation
EEG signal processing is often time-consuming when performed manually, making the process cumbersome in clinical applications. By implementing machine learning models, the diagnosis time can be greatly reduced, leading to improved clinical decision-making and timely interventions.

Approach
The project explores the use of multiple machine learning models, including:

Random Forest (RF)
Support Vector Machine (SVM)
Multilayer Perceptron (MLP)
Preprocessing techniques and feature extraction methods were applied to enhance model performance. Metrics like accuracy and F1-score were used for evaluation.

Dataset
The dataset contains six categories of EEG recordings: GPD, GRDA, Seizure, LPD, LRDA, and Others. The dataset is imbalanced, with under-representation of some patterns like LPD. Various preprocessing steps were undertaken to normalize and prepare the data for classification.

Preprocessing Steps:
Data normalization
Label encoding for categorical data
Feature extraction in time, frequency, and wavelet domains
Models and Methodology
Three models were implemented:

Random Forest (RF):
Number of Trees: 500
Test Accuracy: 83.42%
Support Vector Machine (SVM):
Kernel: Radial Basis Function (RBF)
Test Accuracy: 90.5%
Multilayer Perceptron (MLP):
Hidden Layers: (128, 64, 32)
Test Accuracy: 88.83%
Results
The SVM model outperformed the others with the highest accuracy of 90.5%.
The MLP model demonstrated strong adaptability to complex patterns.
The Random Forest model offered interpretability but struggled with minor class representation.
Challenges
Memory Constraints: The dataset size (26.4 GB) led to computational limitations, requiring smaller batch sizes.
Class Imbalance: Certain EEG patterns like LRDA were underrepresented, making classification difficult.
Feature Extraction Bottlenecks: The large dataset and the complexity of features required significant computational resources.
Conclusion
SVM emerged as the best-performing model for EEG-based classification, making it a suitable candidate for clinical use. While Random Forest provided explainability, the MLP model showed promise for future applications with larger datasets.

Future Work
Address dataset imbalance through data augmentation.
Explore deep learning approaches like Convolutional Neural Networks (CNN) for improved accuracy.
