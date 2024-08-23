# Driver Seat-Belt Detection Using CNN-SVM Hybrid Approach

This project focuses on developing an efficient system to detect if a driver is wearing a seat belt using a hybrid Convolutional Neural Network (CNN) and Support Vector Machine (SVM) classifier. The proposed model analyzes images to determine if a seat belt is buckled, leveraging the feature extraction capabilities of CNN and the classification strength of SVM.


# Project Overview
Seat belt detection is crucial in transportation systems to reduce accidents and ensure safety. Traditional sensor-based methods are often bypassed, leading to inconsistent seat belt usage. This project aims to enhance detection accuracy using image processing and machine learning techniques.

# Key Features
Hybrid Model: Combines CNN for feature extraction and SVM for binary classification, achieving higher accuracy.
Data Augmentation: Utilizes techniques like rescaling, shearing, zooming, and horizontal flipping to improve model robustness.
Training and Evaluation: The model is trained on a dataset with a train-validation-test split of 70%-20%-10%, and evaluated using accuracy, loss, and confusion matrix.

# Dataset
The dataset used in this project includes images categorized into two classes: "seat belt" and "no seat belt". The images are preprocessed and resized to 64x64 pixels.

Training Set: 70% of the dataset
Validation Set: 20% of the dataset
Test Set: 10% of the dataset
# Model Architecture
## The CNN-SVM model architecture is as follows:
Convolutional Layers: Two convolutional layers with ReLU activation and max-pooling for feature extraction.
Flattening: Converts the pooled feature maps into a single vector.
Dropout Layers: Prevents overfitting by randomly setting input units to 0.
Fully Connected Layer: Dense layer with ReLU activation.
Output Layer: A Dense layer with a linear activation function for binary classification.

# Training
The model is compiled using the Adam optimizer and hinge loss function. It is trained for 20 epochs, and the performance is evaluated on the validation and test sets.
# Evaluation
The model's performance is visualized using loss and accuracy plots. Additionally, a confusion matrix and classification report are generated to evaluate precision, recall, and F1-score.
