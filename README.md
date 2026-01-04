# Customer Churn Prediction Using Deep Learning
<br>

## Project Overview

Customer churn prediction focuses on identifying customers who are likely to stop using a company’s services.
This project implements an Artificial Neural Network (ANN) using TensorFlow/Keras to predict customer churn based on historical data.

The objective is to build a stable and well-generalized model, not just a high-accuracy one.

## Dataset Description

The dataset contains customer demographic information, service usage details, and billing-related features.


### Key Characteristics

Binary classification problem (Churn / No Churn)

Combination of numerical and categorical features

Target variable: Churn
<br>

<img width="1786" height="551" alt="Screenshot 2026-01-04 152412" src="https://github.com/user-attachments/assets/255ef689-bb23-46cc-a285-ffaa73304d16" />
<img width="838" height="501" alt="Screenshot 2026-01-04 152737" src="https://github.com/user-attachments/assets/cbbc397c-8d39-43e1-beda-0d8663f2c23f" />

<br>
<br>

## Data Preprocessing

Proper preprocessing was applied before training the model.

### Techniques Used

  1. Handling missing values

  2. Encoding categorical variables

  3. Feature scaling using StandardScaler

### Why StandardScaler?

  1. Scales features to mean = 0 and variance = 1

  2. Improves neural network convergence

  3. Prevents features with large ranges from dominating training


<br>
<br>



## Activation Functions

Multiple activation functions were experimented with to improve learning performance.

### ReLU (Rectified Linear Unit)

  a. Faster convergence

  b. Mitigates the vanishing gradient problem

### ELU (Exponential Linear Unit)

  a. Better learning for negative inputs

  b. Smoother gradient flow compared to ReLU





## Weight Initialization Techniques

To stabilize training and improve convergence, the following initialization methods were used:

### Initialization Methods

  1. He Uniform

  2. He Normal

  3. Glorot (Xavier) Uniform

  4. Glorot (Xavier) Normal

Importance of Weight Initialization

Prevents exploding and vanishing gradients

Improves training stability

Helps deeper networks learn efficiently


## Training Configuration

The neural network was trained using the following configuration:

### Training Details

  1. Epochs: 100

  2. Optimizer: Adam

  3. Loss Function: Binary Crossentropy

  4. Evaluation Metric: Accuracy

Early stopping ensured that training stopped at the optimal point.




## Future Improvements

  1. Hyperparameter tuning

  2. Threshold optimization to improve recall

  3. Deployment using Flask or FastAPI

  4. Advanced techniques for class imbalance
