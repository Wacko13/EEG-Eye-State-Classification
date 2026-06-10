# EEG Eye State Classification using Machine Learning

## Overview

This project focuses on the classification of human eye states (Open/Closed) using Electroencephalography (EEG) signals and Machine Learning techniques.

The objective is to analyze EEG sensor data and develop predictive models capable of accurately determining whether a subject's eyes are open or closed. Multiple machine learning algorithms were implemented and compared to identify the most effective model.

---

## Problem Statement

Eye-state detection using EEG signals plays a significant role in:

- Brain-Computer Interfaces (BCI)
- Human-Computer Interaction
- Attention Monitoring Systems
- Assistive Technologies
- Biomedical Signal Processing

The goal of this project is to build and evaluate machine learning models capable of classifying eye states from EEG measurements.

---

## Dataset Information

The dataset consists of EEG recordings collected from 14 sensors placed on the scalp.

### Dataset Statistics

| Attribute | Value |
|------------|---------|
| Total Samples | 14,980 |
| Features | 14 EEG Channels |
| Classes | Open Eyes (0), Closed Eyes (1) |

### EEG Channels

- AF3
- F7
- F3
- FC5
- T7
- P7
- O1
- O2
- P8
- T8
- FC6
- F4
- F8
- AF4

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- TensorFlow / Keras

---

## Project Workflow

### 1. Data Loading
- Dataset extraction and loading
- Data inspection and validation

### 2. Data Preprocessing
- Missing value analysis
- Feature selection
- Data normalization using StandardScaler

### 3. Dataset Splitting
- Training Set: 80%
- Testing Set: 20%

### 4. Machine Learning Models

#### Neural Network
- Dense Neural Network Architecture
- ReLU Activation
- Sigmoid Output Layer
- Adam Optimizer

#### Random Forest Classifier
- Ensemble Learning Approach
- Multiple Decision Trees
- Robust Classification Performance

#### Support Vector Machine (SVM)
- Margin-Based Classification
- High-Dimensional Feature Analysis

---

## Model Performance

| Model | Accuracy |
|---------|----------|
| Neural Network | 66.69% |
| Support Vector Machine (SVM) | 61.31% |
| Random Forest Classifier | **92.46%** |

### Best Performing Model

🏆 **Random Forest Classifier**

The Random Forest model achieved the highest classification accuracy of **92.46%**, significantly outperforming the Neural Network and SVM models.

---

## Visualizations

The project includes:

- Accuracy vs Epoch Graph
- Loss vs Epoch Graph
- Model Comparison Graph
- Confusion Matrix
- ROC Curve

These visualizations provide a comprehensive evaluation of model performance and classification capability.

---

## Prediction Demonstration

A prediction module was implemented to:

- Select EEG samples
- Predict eye state
- Display prediction probabilities
- Compare actual and predicted labels

Example Output:

| Actual Class | Predicted Class | Open Probability (%) | Closed Probability (%) |
|-------------|----------------|----------------------|-----------------------|
| 0 | 0 | 53.5 | 46.5 |

---

## Results and Analysis

The comparison of multiple machine learning models revealed that ensemble-based approaches are highly effective for EEG signal classification.

Key findings:

- Random Forest achieved superior performance.
- Neural Networks provided moderate classification accuracy.
- SVM showed comparatively lower performance on this dataset.
- Ensemble learning techniques proved more suitable for this EEG classification task.

---

## Future Improvements

- Hyperparameter Optimization
- XGBoost Implementation
- Deep Learning Architectures (CNN/LSTM)
- Real-Time EEG Signal Processing
- Brain-Computer Interface Integration
- Web-Based Deployment

---

## Repository Structure

```

EEG-Eye-State-Classification/
│
├── model(eeg).ipynb
├── README.md
├── requirements.txt
├── dataset/
│   └── EEG_Eye_State_Classification.csv
│
└── images/
├── accuracy_curve.png
├── confusion_matrix.png
├── roc_curve.png
└── model_comparison.png

```

---

## Author

**Shreyash**
B.Tech Electronics & Computer Engineering (ECM)

Interested in:
- Machine Learning
- Artificial Intelligence

---

## License

This project is developed for educational and research purposes.
