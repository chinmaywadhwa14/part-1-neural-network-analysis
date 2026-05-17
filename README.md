# Part 1: Neural Network Fundamentals and Training Behavior Analysis

## Project Overview

This project focuses on building and analyzing a simple Artificial Neural Network (ANN) for customer churn prediction using TensorFlow and Keras.

The objective of this assignment is not only to train a neural network model, but also to understand how neural networks learn through:
- forward propagation
- activation functions
- loss calculation
- backpropagation
- parameter optimization

The dataset contains customer-related features such as contract type, payment method, monthly charges, support tickets, satisfaction score, and usage behavior.

The target variable used for prediction is:
- `churn`
  - 0 → Customer stays
  - 1 → Customer leaves

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras

---

# Tasks Performed

## 1. Dataset Understanding
- Loaded and explored the dataset
- Checked shape and column information
- Verified missing values
- Generated statistical summaries
- Visualized target variable distribution

## 2. Data Preprocessing
- Encoded categorical features
- Split dataset into training and testing sets
- Applied feature scaling using StandardScaler

## 3. Neural Network Model Building
The ANN model includes:
- Input Layer
- Hidden Layer 1 → 16 neurons (ReLU)
- Hidden Layer 2 → 8 neurons (ReLU)
- Output Layer → 1 neuron (Sigmoid)

Optimizer Used:
- Adam

Loss Function:
- Binary Crossentropy

---

# Model Training and Evaluation

The model was trained using:
- Epochs: 20
- Batch Size: 32

Evaluation techniques used:
- Accuracy score
- Classification report
- Confusion matrix
- Accuracy visualization graph

---

# Hyperparameter Experimentation

Different configurations were tested by changing:
- Number of hidden layers
- Number of neurons
- Learning rate

The comparison results are stored in:
- `results/model_comparison_table.csv`

---

# Observations

- The model achieved high accuracy on the test dataset.
- The dataset is highly imbalanced because non-churn customers are much higher than churn customers.
- Due to class imbalance, the model performed better for non-churn predictions compared to churn predictions.

---

# Repository Structure

```text
part-1-neural-network-analysis/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
│
└── results/
    ├── model_comparison_table.csv
    └── evaluation_outputs.png
```

---

# Conclusion

This project helped in understanding:
- neural network fundamentals
- preprocessing techniques
- model training behavior
- evaluation metrics
- hyperparameter tuning

It also provided practical experience in implementing ANN models using TensorFlow and Keras.
