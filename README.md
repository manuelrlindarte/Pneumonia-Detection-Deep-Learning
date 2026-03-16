# Pneumonia Detection using Deep Learning

This project develops a deep learning model capable of detecting pneumonia from chest X-ray images using Convolutional Neural Networks and Transfer Learning.

The objective is to evaluate the potential of deep learning models as a support tool for medical image classification.

---

## Problem Statement

Pneumonia is a serious respiratory disease that can be identified through chest X-ray images. However, manual diagnosis requires trained radiologists and can be time-consuming.

Deep learning models have shown strong performance in medical image classification tasks. In this project, a convolutional neural network was trained to automatically classify chest X-ray images into two categories:

- Normal
- Pneumonia

---

## Dataset

The dataset used contains pediatric chest X-ray images labeled as **Normal** or **Pneumonia**.

The dataset includes:

- Training images
- Validation images
- Test images

These images were collected from the Guangzhou Women and Children’s Medical Center.

---

## Methodology

The project follows a typical machine learning workflow:

1. Data exploration and preprocessing
2. Image normalization and resizing
3. Train / validation / test split
4. Model selection
5. Model training
6. Model evaluation

---

## Model Architecture

Transfer learning was applied using **VGG16**, a pre-trained convolutional neural network originally trained on ImageNet.

Steps applied:

- Load VGG16 base model
- Freeze initial convolutional layers
- Add custom dense layers for classification
- Fine-tune higher layers of the network

This approach allows the model to leverage previously learned visual features while adapting to the pneumonia classification task.

---

## Evaluation Metrics

The model performance was evaluated using:

- Accuracy
- Confusion Matrix
- ROC Curve
- AUC score

These metrics allow assessing both classification accuracy and the model's ability to distinguish between classes.

---

## Results

The trained model achieved strong predictive performance in identifying pneumonia cases.

Main results include:

- High classification accuracy
- Strong AUC score
- Good separation between Normal and Pneumonia classes

Example evaluation results are shown below.

---

## Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

---

## ROC Curve

![ROC Curve](images/roc_curve.png)

---

## Repository Structure
