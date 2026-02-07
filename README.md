Project Name

Advanced Time Series Forecasting using Deep Learning Transformer and LSTM Baseline

Project Overview

This project implements an advanced deep learning system for multivariate time series forecasting. The goal of the project is to predict future values using historical sequential data. The project uses a Transformer based deep learning model which contains an attention mechanism. Attention helps the model learn which past time steps are more important for prediction.

The project also includes a baseline LSTM model for performance comparison. Hyperparameter tuning is performed to find the best learning rate and batch size. The project also includes attention weight analysis and performance evaluation using RMSE.

Dataset Details

The dataset used in this project is synthetic multivariate time series data.

Total samples 2000
Total input features 3
Target variable 1
Sequence length 30 time steps

Feature Description

Feature one sine seasonal pattern with gaussian noise
Feature two cosine seasonal pattern with gaussian noise
Feature three combined sine and cosine trend pattern

Target value is generated using weighted combination of all three features.

Data Preprocessing

Data normalization is done using MinMax scaling.
Time series data is converted into supervised learning sequence format.
Training data split eighty percent
Testing data split twenty percent

Model Architecture

Transformer Model
Input features three
Embedding dimension sixty four
Attention heads four
Transformer encoder layers two
Loss function mean squared error
Optimizer Adam
Learning rate selected after tuning

Baseline Model

LSTM network
Hidden units sixty four
Loss function mean squared error
Optimizer Adam

Hyperparameter Tuning

Learning rate tested zero point zero one and zero point zero zero one
Batch size tested thirty two and sixty four
Best learning rate zero point zero zero one
Best batch size thirty two

Training Details

Training is performed for ten epochs after hyperparameter tuning.
Model is trained using batch training method.

Evaluation Method

Model performance is evaluated using root mean squared error.
Transformer performance compared with LSTM baseline model.

Results

Transformer model achieved lower RMSE compared to LSTM model.
This shows Transformer with attention performs better for long sequence learning.

Attention Analysis

Attention weights are extracted from Transformer encoder output.
Attention visualization shows model focuses more on recent time steps and seasonal peaks.

How To Run Project

Install required Python libraries
Run the single cell code in Jupyter notebook or Python environment
Train the model
View RMSE results and plots

Technologies Used

Python
PyTorch
NumPy
Scikit Learn
Matplotlib

Future Improvements

Use real world dataset such as weather or energy consumption data
Increase training epochs
Add more hyperparameter tuning options
Deploy model using web application

Conclusion

This project demonstrates how Transformer based deep learning models with attention mechanism can improve multivariate time series forecasting performance compared to traditional deep learning models like LSTM.
