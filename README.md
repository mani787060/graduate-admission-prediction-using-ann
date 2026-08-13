# 🎓 Graduate Admission Prediction Using Artificial Neural Network

## 📌 Project Overview

This project develops an **Artificial Neural Network (ANN)** to predict the probability of a student being admitted to a graduate program based on their academic performance and profile.

The model learns relationships between factors such as **GRE score, TOEFL score, CGPA, university rating, statement of purpose, letter of recommendation, and research experience** to estimate a candidate's admission probability.

This project demonstrates how **Deep Learning can be applied to a real-world regression problem**.

---

## 🎯 Objective

The primary objective is to build a regression model that predicts the **Chance of Admit** for a graduate applicant.

The predicted value ranges between approximately `0` and `1`, where a higher value represents a greater estimated probability of admission.

---

## 📊 Dataset

The project uses the **Graduate Admissions** dataset.

**Dataset file:**

```text
Admission_Predict_Ver1.1.csv
```

### Features

| Feature           | Description                                   |
| ----------------- | --------------------------------------------- |
| GRE Score         | Graduate Record Examination score             |
| TOEFL Score       | TOEFL examination score                       |
| University Rating | Rating of the applicant's university          |
| SOP               | Strength of Statement of Purpose              |
| LOR               | Strength of Letter of Recommendation          |
| CGPA              | Undergraduate CGPA                            |
| Research          | Whether the candidate has research experience |

### Target Variable

**Chance of Admit**

A continuous value representing the estimated probability of admission.

---

## 🧠 Problem Type

This is a **Supervised Learning Regression Problem**.

Unlike classification, the model does not predict a fixed category. Instead, it predicts a continuous numerical value representing the admission probability.

---

## 🔄 Project Workflow

The project follows a complete Deep Learning workflow:

```text
Dataset
   ↓
Data Loading & Inspection
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
ANN Architecture
   ↓
Model Training
   ↓
Validation
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 🧹 Data Preprocessing

Before training the ANN, the dataset is prepared through several preprocessing steps:

* Load and inspect the dataset
* Check data types and missing values
* Separate input features and target variable
* Split the dataset into training and testing sets
* Scale numerical features

### Why Feature Scaling?

ANNs are sensitive to differences in feature magnitude. Scaling the input features helps the optimization process converge more efficiently and prevents features with larger numerical ranges from dominating the learning process.

---

## 🧠 ANN Architecture

The project uses a **Feedforward Artificial Neural Network** for regression.

### Architecture

```text
Input Features
      ↓
Dense Layer
      ↓
ReLU Activation
      ↓
Dense Layer
      ↓
ReLU Activation
      ↓
Output Layer
      ↓
Predicted Admission Probability
```

### Hidden Layers

The hidden layers use the **ReLU (Rectified Linear Unit)** activation function to introduce non-linearity and allow the network to learn complex relationships between the input features and admission probability.

### Output Layer

The output layer contains a **single neuron** because the task involves predicting one continuous target value.

---

## Model Training

The neural network is trained using:

* Forward propagation
* Backpropagation
* Gradient-based optimization
* Regression loss
* Multiple training epochs

During training, the model adjusts its weights to minimize the difference between the predicted and actual admission probabilities.

---

## Model Evaluation

The ANN is evaluated using multiple regression metrics.

### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted values.

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted values.

### R² Score

Measures how well the model explains the variation in the target variable.

Using multiple metrics provides a more complete understanding of model performance.

---

## Key Learning

This project demonstrates that Artificial Neural Networks are not limited to classification problems.

They can also be used for **regression tasks**, where the objective is to predict continuous numerical values.

The project also highlights the importance of:

* Feature scaling
* Appropriate model architecture
* Activation functions
* Train-test splitting
* Regression metrics
* Model validation

---

## Practical Use Case

A system like this could help students understand how different academic and profile factors relate to graduate admission outcomes.

For example, an applicant could provide their academic profile and receive an estimated admission probability from the trained model.

> **Note:** Such predictions should be treated as estimates rather than guaranteed admission decisions because real admission decisions depend on many factors that may not be present in the dataset.

---

## Technologies Used

### Programming Language

* Python

### Libraries & Frameworks

* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* TensorFlow
* Keras

### Development Environment

* Jupyter Notebook
* Kaggle Notebook

---

## Project Structure

```text
graduate-admission-prediction-using-ann/
│
├── graduate-admission-prediction-using-ann.ipynb
├── README.md
└── Admission_Predict_Ver1.1.csv
```

> The dataset can also be loaded directly from the Kaggle environment.

---

## Learning Outcomes

Through this project, I gained practical experience with:

* Regression problems
* Artificial Neural Networks
* Data preprocessing
* Feature scaling
* Train-test splitting
* Dense neural network layers
* ReLU activation
* Regression output layers
* Model training
* Backpropagation
* MSE and MAE
* R² evaluation
* Applying Deep Learning to real-world prediction problems

---

## Future Improvements

Potential improvements include:

* Hyperparameter tuning
* Experimenting with different ANN architectures
* Adding Dropout regularization
* Implementing Early Stopping
* Learning-rate optimization
* Comparing ANN with Linear Regression
* Comparing ANN with Random Forest and XGBoost
* Feature importance and interpretability analysis
* Cross-validation
* Building an interactive prediction application
* Deploying the model using Streamlit or FastAPI

---

## Final Takeaway

This project demonstrates how an **Artificial Neural Network can be used to solve a real-world regression problem by learning relationships between academic/profile features and graduate admission probability**.

It provides practical experience with the complete Deep Learning workflow—from data preprocessing and feature scaling to ANN architecture design, model training, prediction, and evaluation.

The project also serves as a foundation for exploring more advanced **Deep Learning, model optimization, and explainable AI techniques**.
