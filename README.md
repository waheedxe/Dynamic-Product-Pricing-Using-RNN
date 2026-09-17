# Dynamic Product Pricing Prediction Using RNN & LSTM

## Project Overview
This deep learning project focuses on **Dynamic Product Pricing Prediction** using two recurrent neural-network architectures: **Simple RNN** and **LSTM**.

The **Simple RNN** was developed as the main capstone model. An **LSTM (Long Short-Term Memory)** model was later implemented as an additional experiment to check whether prediction performance could be improved.

## Objective
The objective is to predict product prices from sequentially prepared business data and compare the predictive performance of recurrent deep-learning models for a regression problem.

## Models Implemented

### 1. Simple RNN — Main Capstone Model
The main capstone model uses a **Simple Recurrent Neural Network (SimpleRNN)**.

The workflow includes:
- Loading and understanding the dataset
- Data preprocessing
- Preparing sequential input
- Building and training the Simple RNN model
- Generating predictions
- Evaluating regression performance
- Comparing the RNN against a baseline model

### RNN Performance

| Metric | Result |
| --- | ---: |
| MAE | 19.88 |
| MSE | 724.49 |
| RMSE | 26.92 |
| R² Score | 0.5294 (~52.94%) |

The RNN achieved an R² score of approximately **0.53**, indicating moderate predictive performance on the test data.

### RNN vs Baseline
The baseline model produced approximately:
- **R²:** -0.0004
- **MAE:** 32.83
- **RMSE:** 39.25

The RNN therefore performed substantially better than the mean-based baseline model.

---

### 2. LSTM — Additional Experiment
An **LSTM model** was implemented after the RNN model to test whether a more advanced recurrent architecture could improve prediction performance.

The LSTM experiment includes:
- Sequential data preparation
- Data scaling
- LSTM layer with 64 units
- Dense layer with 32 units
- Regression output layer
- Early Stopping
- Prediction and inverse transformation
- Regression evaluation
- Actual vs predicted price visualization

### LSTM Training Configuration
- Maximum epochs: **40**
- Batch size: **32**
- Validation split: **20%**
- Early stopping patience: **5**
- Total model parameters: **20,289**

### LSTM Performance

| Metric | Result |
| --- | ---: |
| MAE | 11.17 |
| RMSE | 16.14 |
| R² Score | 0.8307 (~83.07%) |

The LSTM achieved an R² score of approximately **0.83**, showing stronger predictive performance than the Simple RNN in these experiments.

## Model Comparison

| Model | MAE | RMSE | R² Score |
| --- | ---: | ---: | ---: |
| Simple RNN | 19.88 | 26.92 | 0.5294 |
| LSTM | 11.17 | 16.14 | 0.8307 |

In the recorded notebook results, the **LSTM produced lower prediction errors and a higher R² score than the Simple RNN**.

## Evaluation Metrics
- **MAE (Mean Absolute Error):** Average absolute difference between actual and predicted prices.
- **MSE (Mean Squared Error):** Average squared prediction error.
- **RMSE (Root Mean Squared Error):** Prediction error expressed in the target's original scale.
- **R² Score:** Measures how much variation in product prices is explained by the model.

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Simple RNN
- LSTM

## Repository Structure
```text
Dynamic-Product-Pricing-Using-RNN/
├── Dynamic Product Pricing using RNN.ipynb
├── Dynamic Product Pricing Using LSTM.ipynb
├── sales_data.csv
└── README.md
```

## How to Run
1. Clone or download this repository.
2. Open either notebook in Jupyter Notebook.
3. Install the required Python libraries.
4. Keep `sales_data.csv` accessible to the notebooks or update the dataset path if necessary.
5. Run the notebook cells in sequence.

## Project Type
**Deep Learning – RNN & LSTM – Regression**

## Author
**Waheed Bepari**

**Main capstone model:** Simple RNN  
**Additional performance experiment:** LSTM
