# vulnerability-detection-using-machine-learning

This project aims to detect vulnerabilities using various machine learning models. The models used in this project include Random Forest, Support Vector Machine (SVM), Neural Network, and k-Nearest Neighbors (k-NN). The goal is to predict the impact scores of vulnerabilities accurately.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Data Description](#data-description)
- [Methods](#methods)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Overview
In this project, we explore different machine learning algorithms to predict the impact scores of vulnerabilities. The performance of each model is evaluated using Mean Squared Error (MSE) and Mean Absolute Error (MAE).

## Installation
To run this project, you need to have Python installed along with the following libraries:
- pandas
- numpy
- scikit-learn
- tensorflow
- keras
- matplotlib
- seaborn

You can install the required libraries using pip:

```bash
pip install pandas numpy scikit-learn tensorflow keras matplotlib seaborn
```
### Data Description
The dataset used in this project is sourced from the National Vulnerability Database (NVD) and is called nvdcve-1.1-2003.json. It consists of various features related to vulnerabilities. The target variable is the impact score, which we aim to predict.

### Methods
The following machine learning models were implemented and compared:

- Random Forest
- Support Vector Machine (SVM)
- Neural Network
- k-Nearest Neighbors (k-NN)
- Data Preprocessing
- The data was preprocessed by handling missing values, encoding categorical variables, and normalizing the features.

### Model Training
Each model was trained using a portion of the dataset, and their performances were evaluated on a test set.

### Performance Metrics
The models were evaluated using the following metrics:

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)

------------

### Results:

The performance of the models was as follows:

**Random Forest:**

MSE: 2.845
MAE: 1.290
SVM:

MSE: 3.465
MAE: 1.423

**Neural Network:**

MSE: 5.337
MAE: 1.777
k-NN:

MSE: 4.294
MAE: 1.596

------------


### Interpretation:
**The Random Forest model** had the best performance with the lowest MSE and MAE, indicating higher accuracy in predicting vulnerability impact scores.
The SVM model showed slightly lower performance compared to Random Forest, with higher MSE and MAE.

**The k-NN model** had intermediate performance, with errors higher than Random Forest and SVM but lower than the Neural Network.
The Neural Network had the highest errors, indicating the lowest accuracy in predictions.

### Conclusion
The Random Forest model was the most effective in predicting the impact scores of vulnerabilities, followed by SVM and k-NN. The Neural Network model performed the worst in this context.

