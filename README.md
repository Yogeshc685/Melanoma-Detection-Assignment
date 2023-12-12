# Skin Cancer Classification Project

## Abstract

Cancer manifests in diverse forms, with melanoma standing out as the most lethal type of skin cancer. The diagnostic journey for melanoma involves clinical screening, dermoscopic analysis, and histopathological examination. Timely identification at early stages significantly enhances the curability of melanoma skin cancer. The initial step in diagnosis entails visually examining the affected skin area. Dermatologists employ high-speed cameras to capture dermatoscopic images of skin lesions, achieving a diagnostic accuracy of 65-80%. Further assessment by cancer treatment specialists raises the overall prediction rate to 75-84%. This project aims to construct an automated classification system, leveraging image processing techniques for the categorization of skin cancer using lesion images.

## Problem Statement

The conventional skin biopsy process involves dermatologists extracting a portion of the skin lesion and scrutinizing it under a microscope, a procedure spanning nearly a week. This project seeks to reduce this timeframe to a mere couple of days by introducing a predictive model. The approach relies on Convolutional Neural Networks (CNN) to classify nine types of skin cancer from outlier lesion images, potentially positively impacting millions of lives.

## Motivation

The overarching objective is to contribute to the reduction of skin cancer-related fatalities. The primary impetus behind the project is to harness advanced image classification technology for the betterment of individuals. The advancements in machine learning and deep learning within the realm of computer vision present scalable solutions applicable across diverse domains.

## Dataset

The dataset encompasses 2357 images of malignant and benign oncological diseases, sourced from the International Skin Imaging Collaboration (ISIC). Images are categorized based on ISIC criteria, and subsets are evenly divided. The dataset includes various diseases such as `datasetdf` and `datasetplot`. To address class imbalance, the Augmentor Python package was utilized to augment samples across all classes.



## CNN Architecture Design

In the pursuit of skin cancer classification using lesion images, a custom CNN model has been devised to attain superior accuracy and results in the classification task.

- **Rescaling Layer:** Converts input pixel values from the [0, 255] range to the [0, 1] range.
- **Convolutional Layer:** Applies a convolution operation to the input, condensing the image size and consolidating information.
- **Pooling Layer:** Reduces feature map dimensions, minimizing parameters and computational load.
- **Dropout Layer:** Mitigates overfitting by randomly setting input units to 0 during training.
- **Flatten Layer:** Converts the output to a 1-dimensional array for input to the next layer.
- **Dense Layer:** A deeply connected neural network layer where each neuron receives input from all neurons of its preceding layer.
- **Activation Function(ReLU):** Overcomes the vanishing gradient problem, facilitating faster learning.
- **Activation Function(Softmax):** Employed in the output layer for predicting a multinomial probability distribution.



## Model Evaluation

Accuracy
