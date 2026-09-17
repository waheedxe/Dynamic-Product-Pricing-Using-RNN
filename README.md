# Dynamic Product Pricing Prediction Using RNN

## Project Overview
This deep learning project predicts product prices using a Recurrent Neural Network (RNN). It was developed as a capstone project to apply deep learning to a regression problem and evaluate how effectively an RNN can learn patterns from sequentially prepared pricing data.

## Objective
The objective is to build and evaluate an RNN-based model for predicting product prices from the available features in the dataset.

## Approach
The project workflow includes:

1. Loading and understanding the dataset
2. Data preprocessing and preparation
3. Preparing sequential input for the RNN
4. Building a Simple RNN model
5. Training the model
6. Generating predictions
7. Evaluating regression performance
8. Comparing model predictions with actual values

## Deep Learning Model
The project uses a **Simple Recurrent Neural Network (SimpleRNN)** as the main deep learning approach.

The network includes:
- SimpleRNN layer
- Dropout for regularization
- Dense layers
- Regression output layer

## Evaluation Metrics
Model performance is evaluated using common regression metrics:

- **MAE (Mean Absolute Error)** – average absolute prediction error
- **MSE (Mean Squared Error)** – average squared prediction error
- **RMSE (Root Mean Squared Error)** – prediction error expressed in the original target scale
- **R² Score** – indicates how much variation in product prices is explained by the model

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Recurrent Neural Network (RNN)

## Repository Structure
```text
Dynamic-Product-Pricing-Using-RNN/
├── Dynamic Product Pricing using RNN(1).ipynb
├── dataset.csv
└── README.md
```

> Rename `dataset.csv` above to the actual dataset filename when uploading it.

## How to Run
1. Clone or download this repository.
2. Open the Jupyter Notebook.
3. Make sure the required Python libraries are installed.
4. Update the dataset path if necessary.
5. Run the notebook cells in order.

## Project Type
**Deep Learning – Regression**

## Author
**Waheed Bepari**

Capstone Project
