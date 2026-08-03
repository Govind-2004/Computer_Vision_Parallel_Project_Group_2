# Brain Tumor MRI Classification using Deep Learning

## Overview

This project presents a comprehensive workflow for **multi-class brain tumor classification** using **Convolutional Neural Networks (CNN)** and **Transfer Learning (VGG16)** on MRI brain images.

The project focuses on loading and preprocessing MRI images, performing exploratory data analysis (EDA), developing deep learning models, evaluating their performance, and comparing a custom CNN with a pre-trained VGG16 model for accurate brain tumor classification.

The models classify MRI images into one of the following categories:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

**Dataset Source:** https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data

---

# Project Structure

## 1. Libraries

- Import required Python libraries
- Configure visualization settings
- Load TensorFlow, OpenCV, NumPy and Matplotlib libraries

---

## 2. Dataset Loading

- Mount Google Drive
- Verify dataset folder structure
- Load training, validation and testing datasets
- Display class names
- Count images in each class

---

# Dataset Information

The dataset contains MRI images categorized into **four classes** for multi-class brain tumor classification.

| Class | Description |
|---------|-------------|
| **Glioma** | MRI images containing Glioma tumors |
| **Meningioma** | MRI images containing Meningioma tumors |
| **Pituitary** | MRI images containing Pituitary tumors |
| **No Tumor** | MRI images without any tumor |

### Dataset Distribution

Training Dataset

- Glioma – 1400 Images
- Meningioma – 1400 Images
- Pituitary – 1400 Images
- No Tumor – 1410 Images

Testing Dataset

- Glioma – 403 Images
- Meningioma – 400 Images
- Pituitary – 400 Images
- No Tumor – 401 Images

---

# Exploratory Data Analysis (EDA)

### Dataset Verification

- Verify image loading
- Verify class labels
- Display sample MRI images
- Check image dimensions

### Dataset Analysis

- Count images per class
- Visualize class distribution
- Verify balanced dataset

---

# Data Preprocessing

## Image Processing

- Create Validation Dataset
- Resize images
- Normalize pixel values
- Batch images
- Shuffle training dataset

## Data Augmentation

The following augmentation techniques were applied:

- Random Flip
- Random Rotation
- Random Zoom

Data augmentation improves model generalization and reduces overfitting.

---

# Deep Learning Models

The following deep learning models were implemented:

- Convolutional Neural Network (CNN)
- VGG16 Transfer Learning Model

---

# Custom CNN Architecture

The custom CNN consists of:

- Convolution Layers
- MaxPooling Layers
- Dropout Layer
- Dense Layer
- Softmax Output Layer

---

# Model Training

Both models were trained using:

- Adam Optimizer
- Sparse Categorical Crossentropy Loss
- Accuracy Metric

Training improvements included:

- Early Stopping
- Model Checkpoint
- Validation Dataset Monitoring

---

# Model Evaluation

The models were evaluated using:

- Training Accuracy
- Validation Accuracy
- Test Accuracy
- Training Loss
- Validation Loss
- Test Loss

Performance curves included:

- Accuracy vs Epoch
- Loss vs Epoch

Random MRI image prediction was also performed on unseen test images.

---

# Prediction

The trained models were used to:

- Load a random MRI image from the testing dataset
- Predict the tumor class
- Display the actual class
- Display the predicted class
- Display prediction confidence
- Visualize the prediction on the MRI image

---

# Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Google Colab

---

# Instructions to Run the Project

1. Clone this repository.
2. Download the Brain Tumor MRI Dataset from Kaggle.
3. Upload the dataset to Google Drive.
4. Update the dataset path in the notebook.
5. Run the notebook cells sequentially.
6. The notebook performs:
   - Dataset Loading
   - Exploratory Data Analysis
   - Data Preprocessing
   - Data Augmentation
   - Custom CNN Model Training
   - VGG16 Transfer Learning
   - Model Evaluation
   - Brain Tumor Prediction

---

# Contributors

| Team Member | Contribution |
|-------------|--------------|
| **Govind Vijay** | Dataset collection, dataset verification, dataset loading, exploratory data analysis (EDA), validation dataset creation, image preprocessing, image normalization, data augmentation, and project documentation. |
| **Aathil** | Custom CNN model development, VGG16 transfer learning model, model compilation, model training, model evaluation, model saving/loading, prediction system, and performance comparison. |

---

# Repository Structure

```text


├── Brain_Tumor_MRI_Classification.ipynb
├── README.md
└── LICENSE
```

---

# Dataset Source

**Brain Tumor MRI Dataset**

Kaggle

https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data
