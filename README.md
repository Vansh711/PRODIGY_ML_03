# Cats vs Dogs Image Classification using Support Vector Machine (SVM)

## Project Overview

This project implements a Support Vector Machine (SVM) classifier to distinguish between images of cats and dogs. The objective is to build an image classification model by preprocessing image data, extracting meaningful features, training an SVM classifier, and evaluating its performance using standard classification metrics.

The project demonstrates the application of traditional machine learning techniques in computer vision and image recognition tasks.

## Dataset

The project uses the Microsoft Cats vs Dogs Dataset available on Kaggle.

Dataset Link:

https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset

The dataset contains thousands of labeled images of cats and dogs used for binary image classification tasks.

To ensure efficient computation in Google Colab, a subset of approximately 8,000 images was used for training and evaluation.

## Technologies Used

* Python
* NumPy
* OpenCV
* Scikit-Learn
* Matplotlib
* Google Colab

## Methodology

### 1. Data Collection

Images were obtained from the Microsoft Cats vs Dogs Dataset available on Kaggle.

### 2. Image Preprocessing

The following preprocessing steps were performed:

* Converted images to grayscale
* Resized images to a fixed size
* Flattened image matrices into feature vectors
* Normalized pixel values
* Applied feature scaling using StandardScaler
* Removed unreadable or corrupted images

### 3. Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

### 4. Model Training

A Support Vector Machine (SVM) classifier was trained using:

* RBF (Radial Basis Function) Kernel
* Feature-scaled image vectors

### 5. Prediction

The trained model was used to classify unseen test images into:

* Cat
* Dog

## Model Evaluation

### Accuracy

**Accuracy:** 82.25%

### Precision

**Precision:** 0.7977

### Recall

**Recall:** 0.9612

### Classification Report

| Class | Precision | Recall | F1-Score |
| ----- | --------- | ------ | -------- |
| Cat   | 0.90      | 0.59   | 0.71     |
| Dog   | 0.80      | 0.96   | 0.87     |

### Overall Performance

| Metric                    | Value  |
| ------------------------- | ------ |
| Accuracy                  | 82.25% |
| Precision                 | 0.7977 |
| Recall                    | 0.9612 |
| Macro Average F1-Score    | 0.79   |
| Weighted Average F1-Score | 0.81   |

## Confusion Matrix Analysis

The confusion matrix indicates that the model performs exceptionally well in identifying dog images while maintaining strong overall classification performance.

### Key Observations

* Most dog images were classified correctly.
* A portion of cat images were incorrectly classified as dogs.
* The model achieved a balanced overall performance with an accuracy exceeding 82%.

## Results

The SVM classifier successfully learned distinguishing patterns between cat and dog images and achieved an overall accuracy of **82.25%** on the test dataset.

Performance improved significantly after:

* Increasing the number of training images
* Normalizing image pixel values
* Applying StandardScaler
* Using the RBF kernel instead of a linear kernel

## Applications

* Animal Image Classification
* Automated Pet Recognition Systems
* Computer Vision Projects
* Image Categorization Tasks
* Machine Learning Education and Research

## Future Improvements

Potential improvements include:

* Using Histogram of Oriented Gradients (HOG) features
* Hyperparameter tuning through GridSearchCV
* Training on the complete dataset
* Implementing Convolutional Neural Networks (CNNs) for higher accuracy

## Conclusion

A Support Vector Machine (SVM) based image classification model was successfully developed to classify cat and dog images. Through image preprocessing, normalization, feature scaling, and kernel optimization, the model achieved an accuracy of **82.25%**.

The project demonstrates that traditional machine learning algorithms can effectively solve image classification problems and provides a strong foundation for more advanced deep learning approaches.

## Author

**Vansh**
B.Tech Computer Science & Engineering (AI & ML)
