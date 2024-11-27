**Overview**

This project focuses on analyzing a Chronic Kidney Disease (CKD) dataset and applying machine learning models for classification tasks. The dataset has been preprocessed to remove inconsistencies, and multiple models, including Naive Bayes, Multilayer Perceptron (MLP), and Radial Basis Function Neural Network (RBFNN), have been implemented to evaluate classification performance.

**Dataset**

The dataset, originally from the UCI Machine Learning Repository, includes clinical data on CKD patients. 



**Objectives**

- Evaluate the performance of different classifiers, including custom architectures.
- Implement and compare models like Naive Bayes, MLP, and RBFNN.
- Perform cross-validation and report key performance metrics.

  
**Project Structure**


1. Naive Bayes Classifier
A Naive Bayes classifier is implemented using the cleaned dataset.
Repeated Random Sampling:
The dataset is split 5 times, with 70% for training and 30% for testing.
Accuracy Results: Average accuracy over multiple runs is reported.

2. Multilayer Perceptron (MLP)
Model Architecture:
Input layer: 24 features.
Hidden layer: 16 neurons with ReLU activation.
Output layer: 1 neuron with sigmoid activation for binary classification.
Training:
Binary Cross-Entropy Loss and Adam optimizer.
Training over 20 epochs using K-Fold Cross-Validation with 5 folds.
Evaluation:
Metrics include accuracy and ROC AUC score for each fold.
Results are averaged across folds.

3. Radial Basis Function Neural Network (RBFNN)
Custom RBF Layer:
Implements a layer with trainable centers and a Gaussian kernel.
Model Architecture:
RBF layer with 10 centers.
Output layer with sigmoid activation for binary classification.
Training:
Binary Cross-Entropy Loss and Adam optimizer.
50 epochs with a 50/50 train-test split.
Evaluation:
Confusion Matrix and Classification Report.

**Results:**

Naive Bayes Classifier
Average accuracy over 5 iterations: ~87%.

Multilayer Perceptron (MLP)
Cross-Validation Results:
Average Accuracy: ~91%.
Average ROC AUC: ~0.92.

Radial Basis Function Neural Network (RBFNN)
Achieved accuracy of ~90% on the test set.

Confusion matrix and detailed classification report indicate balanced performance across classes.
