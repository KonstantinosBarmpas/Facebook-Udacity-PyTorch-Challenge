# **Flower Classifier**

## Project for PyTorch Facebook - Udacity Challenge Scholarship.

---

[network]: ./imgs/Network.png
[overview]: ./imgs/Classifier_Overview.png
[classifier]: ./imgs/Classifier_Explanation.png
[result]: ./imgs/Results30.png

**Introduction**

This is the final project for PyTorch Facebook - Udacity Challenge Scholarship. In this scholarship, 10.000 accepted students will spend 2 months building powerful deep learning models with PyTorch. Top 300 students from the initial challenge course will be selected for the Deep Learning Nanodegree program.

**Files**

This repo contains the main architecture of the model I used, the training and validation data, the notebook with the pytorch code and of course the final model. The model successfully passed the lab assessment for the scholarship.

**Model**

![network]

VGG-19 is an excellent Convolutional Neural Network (CNN) for image classification and I used the pre-trained version that exists in PyTorch models package. After freezing the main features of the network to avoid changes during backpropagation, I replaced the classifier part with my own designed classifier.

![overview]

The classifier is inspired by NVIDIA's neural network used again in Behavioural Cloning Project (check repo) with an added layer of 20588 neurons in the beginning and of course change the number of classes to 102. 

**Training**

During training, I used the pocket algorithm's idea to store and save the model with the minimum validation error to avoid overfitting during unneccesary training steps. The training was done in Udacity's GPU Workspace.

**Results**

![result]

The model had more than >70% accuracy in the validation and successfully passed the PyTorch Facebook - Udacity Scholarship Challenge lab.

---
