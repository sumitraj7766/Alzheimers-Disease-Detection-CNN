# Alzheimer's Disease Detection Using CNN

## Overview
This project uses a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify brain MRI images into four categories: Mild Impairment, Moderate Impairment, No Impairment, and Very Mild Impairment.

The project demonstrates image preprocessing, dataset preparation, CNN model development, and model training and validation.

## Objectives
- Classify brain MRI images into four dataset-defined categories.
- Develop a CNN using TensorFlow and Keras.
- Apply image resizing and pixel normalization.
- Monitor training and validation performance.

## Technology Stack
- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Pillow
- Google Colab

## Dataset
The dataset contains training and testing images organized into four class folders.

| Dataset split | Number of images |
|---|---:|
| Training images | 10,240 |
| Testing images | 1,279 |
| Total | 11,519 |

The training data was divided into 80% training and 20% validation subsets.

Input images were resized to 128 × 128 pixels and normalized to the range [0, 1].

## Model Architecture
The CNN consists of:
- Three convolutional layers with 32, 64, and 128 filters
- Max-pooling layers
- A flattening layer
- A dense layer with 128 neurons
- Dropout with a rate of 0.5
- A four-class softmax output layer

The model was trained using the Adam optimizer and sparse categorical cross-entropy loss for 15 epochs.

## Training Results
At the end of training:

- Training accuracy: 95.21%
- Validation accuracy: 97.07%
- Validation loss: 0.0755

These are training and validation results, not final test-set performance. The held-out test dataset must be evaluated separately before reporting test accuracy.

## How to Run
1. Open the notebook in Google Colab.
2. Obtain the dataset from its original source and arrange the files in the expected directory structure.
3. Update the dataset path in the notebook if necessary.
4. Run the cells sequentially to preprocess the data, build the CNN, and train the model.
5. Evaluate the trained model on the held-out test dataset.

## Limitations
This is an educational machine-learning project. Its predictions are not a medical diagnosis and should not be used for clinical decision-making. Dataset quality, class imbalance, data leakage, and external validation can affect model performance.

## Future Improvements
- Evaluate test accuracy, precision, recall, and F1-score.
- Generate a confusion matrix and classification report.
- Apply data augmentation where appropriate.
- Explore transfer learning with pretrained CNN architectures.
- Investigate model interpretability using Grad-CAM.

## Author
Sumit Kumar

## Disclaimer
This project is intended for educational and research purposes only. It is not a clinically validated diagnostic system.
