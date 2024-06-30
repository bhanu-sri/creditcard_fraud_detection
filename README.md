# Credit Card Fraud Detection

This project aims to build a machine learning model to identify fraudulent credit card transactions. The dataset used in this project is from [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## Table of Contents

- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)


## Dataset

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, with the positive class (frauds) accounting for 0.172% of all transactions.

The features `V1`, `V2`, ..., `V28` are the principal components obtained with PCA, and the only features which have not been transformed with PCA are `Time` and `Amount`. Feature `Time` contains the seconds elapsed between this transaction and the first transaction in the dataset. The feature `Amount` is the transaction Amount, and the feature `Class` is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/creditcard_fraud_detection.git
    ```

2. Change to the project directory:
    ```sh
    cd creditcard_fraud_detection
    ```

## Usage

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

2. Place the downloaded `creditcard.csv` file in the project directory.

3. Run the Jupyter notebook:
    ```sh
    jupyter notebook
    ```

4. Open `credit_card_fraud_detection.ipynb` and run all cells to execute the project steps.

## Model Training and Evaluation

The project follows these steps:

1. **Import Libraries**: Import all necessary libraries for data processing, model training, and evaluation.

2. **Load and Explore Dataset**: Load the dataset and explore its structure and distribution of the target variable.

3. **Pre-process and Normalize the Data**: Handle missing values and normalize the feature data.

4. **Handle Class Imbalance**: Use SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance.

5. **Split the Dataset**: Split the dataset into training and testing sets.

6. **Train a Classification Algorithm**: Train Logistic Regression and Random Forest models.

7. **Evaluate the Model**: Evaluate the models using metrics such as Precision, Recall, and F1-Score.

## Results

The performance of the models is evaluated using the following metrics:

- **Precision**: The ratio of correctly predicted positive observations to the total predicted positives.
- **Recall**: The ratio of correctly predicted positive observations to the all observations in actual class.
- **F1 Score**: The weighted average of Precision and Recall.

The results of the Logistic Regression and Random Forest models are printed in the notebook.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


