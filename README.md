# Early-Detection-of-Potato-Infections
Research on,

# Evaluating CNN and Conventional Machine Learning Approaches for Early Detection of Potato Infections by Alternaria Solani and Phytophthora

## Overview

This project aims to evaluate the effectiveness of Convolutional Neural Networks (CNN) and traditional machine learning models (Support Vector Machine (SVM) and K-Nearest Neighbours (KNN)) for the early detection of potato infections caused by **Alternaria Solani** (early blight) and **Phytophthora infestans** (late blight). The goal is to automate the detection of these diseases using image classification techniques, which can significantly aid in precision agriculture.

## Dataset

The dataset used in this study is publicly available on [Kaggle - PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease). This dataset contains images of various crops, with a focus on potato leaves, categorized into three classes:

- **Healthy potato leaves**
- **Early Blight (Alternaria solani)**
- **Late Blight (Phytophthora infestans)**

### Dataset Details:
- **Healthy**: 152 images
- **Early Blight**: 1,000 images
- **Late Blight**: 1,000 images
- Total images used: **2,152**

## Methodology

### Data Preprocessing:
- All images were resized to **256x256** pixels.
- Data augmentation techniques (rotations, flipping, zooming, etc.) were used on the training data to improve model robustness.
- The dataset was split into training (80%), validation (10%), and test (10%) sets.

### Models Implemented:
1. **Convolutional Neural Network (CNN)**: Deep learning model capable of learning hierarchical image features.
2. **Support Vector Machine (SVM)**: Traditional machine learning algorithm, evaluated using manually extracted features like Histogram of Oriented Gradients (HOG).
3. **K-Nearest Neighbours (KNN)**: Another traditional classifier that relies on the similarity of feature vectors.

### Evaluation Metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**

## Results

The performance of each model was evaluated on the test dataset. Key findings include:
- **CNN**: Achieved **91.7% accuracy** with high precision, recall, and F1-score.
- **SVM**: Achieved **68.3% accuracy**, showing moderate performance.
- **KNN**: Achieved **14.3% accuracy**, demonstrating limitations in handling complex visual classification tasks.

## Conclusion

The study demonstrates the effectiveness of CNN in detecting potato diseases, outperforming traditional machine learning models. CNN’s ability to automatically learn relevant features from image data makes it a powerful tool for early and accurate disease detection in agriculture.

## Getting Started

To run this project locally, follow these steps:

### Prerequisites:
- Python 3.x
- Required libraries (TensorFlow, scikit-learn, etc.)

### Installation:

Clone the repository:

```bash
git clone https://github.com/mdarifhasanbadsha/Early-Detection-of-Potato-Infections.git
cd early-detection-potato-diseases
