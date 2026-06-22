# Vehicle Category Classification Using VGG16 Transfer Learning

## Overview

This project implements a deep learning-based vehicle classification system using the VGG16 Convolutional Neural Network (CNN) architecture and transfer learning techniques. The model is trained to classify vehicle images into five categories:

- Car
- Motorcycle
- Plane
- Ship
- Train

By leveraging pre-trained ImageNet weights, the model is capable of extracting high-level visual features while reducing training time and computational requirements. To improve generalization and robustness, data augmentation techniques such as image rotation, zooming, flipping, brightness adjustment, and shifting were applied during training.

The system is designed to support applications in intelligent transportation systems, traffic monitoring, automated vehicle recognition, and smart city infrastructure.

---

## Features

### Vehicle Classification

- Classifies images into five vehicle categories
- Built using the VGG16 transfer learning architecture
- Generates prediction confidence scores using Softmax

### Data Augmentation

- Rotation
- Zooming
- Horizontal and vertical flipping
- Brightness adjustment
- Width and height shifting
- Shearing transformation

### Deep Learning Pipeline

- Transfer learning using pre-trained VGG16 weights
- Fine-tuning for improved classification performance
- Automatic feature extraction through convolutional layers

### Interactive User Interface

- Gradio-based web application
- Real-time image classification
- User-friendly image upload interface

---

## Dataset

The model was trained using the Vehicle Classification Dataset obtained from Kaggle.

### Vehicle Categories

| Category | Images |
|----------|---------|
| Car | 790 |
| Motorcycle | 800 |
| Plane | 800 |
| Ship | 800 |
| Train | 800 |
| **Total** | **3990** |

The dataset contains vehicle images captured from different viewpoints, lighting conditions, and environments to improve model generalization.

---

## Model Architecture

The classification system utilizes the VGG16 architecture combined with transfer learning.

### Processing Workflow

```text
Input Image
      │
      ▼
Image Preprocessing
      │
      ▼
Data Augmentation
      │
      ▼
VGG16 Feature Extraction
      │
      ▼
Dense Layers
      │
      ▼
Softmax Classification
      │
      ▼
Vehicle Category Prediction
```

### Model Configuration

| Parameter | Value |
|------------|---------|
| Base Model | VGG16 |
| Input Size | 224 × 224 |
| Optimizer | Adam |
| Learning Rate | 0.0001 |
| Loss Function | Categorical Crossentropy |
| Batch Size | 32 |
| Output Classes | 5 |
| Epochs | 22 |

---

## Performance

| Metric | Result |
|---------|---------|
| Training Accuracy | 97% |
| Validation Accuracy | 96% |
| Vehicle Categories | 5 |
| Dataset Size | 3990 Images |

The model achieved strong classification performance across all vehicle categories while maintaining good generalization on unseen images.

---

## Demo Video

To view the complete system demonstration, please download and watch:

```text
Video Project 1.mp4
```

The demonstration showcases:

- Image upload process
- Vehicle classification workflow
- Prediction confidence scores
- User interface functionality
- Real-time inference results

---

## Applications

- Intelligent Transportation Systems
- Vehicle Recognition Systems
- Traffic Monitoring
- Smart City Infrastructure
- Fleet Management
- Transportation Analytics

---

## Future Improvements

- Real-time video classification
- Additional vehicle categories
- Mobile deployment
- Cloud-based inference
- Comparison with ResNet50 and EfficientNet models
- Vehicle detection and tracking integration

---

## Authors

| Name | Student ID |
|--------|------------|
| Revathi A/P Thiyagarajan | A202248 |
| Nancy Anne | A202459 |
| Kavi Priya A/P Balasupramaniam | A202660 |
| Jeslyn A/P A Saminathan | A202747 |

Universiti Kebangsaan Malaysia (UKM)

---

## Built With

**Python • TensorFlow • Keras • VGG16 • Gradio • NumPy • Matplotlib**
