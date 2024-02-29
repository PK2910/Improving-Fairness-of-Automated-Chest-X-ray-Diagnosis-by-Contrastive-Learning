Chest X-ray Contrastive Learning for Bias Mitigation
Overview
Welcome to the Chest X-ray Contrastive Learning project! This initiative aims to employ contrastive learning techniques to mitigate bias in chest X-ray diagnosis. The project focuses on training a model to emphasize the differences between images, thereby reducing biases in medical image predictions.

Table of Contents
Introduction
Dataset
Model Architecture
Contrastive Learning
Training
Results
Usage
Contributing
License
Introduction
Medical diagnoses based on chest X-rays are susceptible to biases stemming from various factors. This project addresses bias mitigation using contrastive learning, which encourages the model to focus on relevant features and reduce biases in learned representations.

Dataset
The dataset used for this project contains chest X-ray images with associated labels. Due to privacy concerns, the dataset is not included in this repository. Please refer to the dataset provider's website for access.

Model Architecture
The model architecture is based on a pre-trained ResNet-18 convolutional neural network. The last fully connected layer of ResNet-18 is replaced with a linear layer tailored to the number of classes in the dataset.

Contrastive Learning
The contrastive learning approach involves training the model on augmented data, encouraging the model to learn representations that minimize intra-class variations and maximize inter-class differences. The loss function used is designed to calculate the contrastive loss based on cosine similarity between the model outputs.

Training
The training process involves augmenting the dataset and optimizing the model using contrastive learning. The training loop iterates over epochs, batches, and augmented images to minimize the contrastive loss.
