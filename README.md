# Graduate Admission Prediction using ANN

## Overview
This project predicts the probability of a student getting admitted to a graduate program using an Artificial Neural Network (ANN).  
The model learns from academic and profile-related features to estimate admission chances.

---

## Objective
To build a deep learning model that predicts admission probability based on a candidate’s academic performance and profile.

---

## Dataset
The dataset contains the following features:
- GRE Score
- TOEFL Score
- University Rating
- SOP Strength
- LOR Strength
- CGPA
- Research Experience

**Target Variable:**
- Chance of Admit (0–1)

---

## Approach
- Data preprocessing and feature scaling
- Train-test split
- ANN model construction using Keras
- Model training and validation
- Performance evaluation using regression metrics

---

## Model Architecture
- Input Layer: Academic profile features
- Hidden Layers: Fully connected Dense layers with ReLU activation
- Output Layer: Single neuron with Sigmoid activation

---

## Evaluation Metrics
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score

---

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- TensorFlow / Keras
- Scikit-learn

---

## Future Enhancements
- Hyperparameter tuning
- Feature importance analysis
- Compare ANN with Linear Regression
- Add dropout to reduce overfitting


