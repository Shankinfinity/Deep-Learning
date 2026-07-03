Traffic Volume Prediction (LSTM)

Overview

This project predicts hourly interstate traffic volume using a deep learning LSTM model built in PyTorch. The dataset (from the UCI Machine Learning Repository) includes weather conditions, holidays, and time features for an interstate highway in Minnesota.

Workflow


Data – load pre-normalized train_scaled.csv / test_scaled.csv.
Sequencing – convert data into 12-hour input sequences to predict the next hour's traffic volume.
Model – a 2-layer LSTM followed by a LeakyReLU and a linear output layer.
Training – trained for 3 epochs using MSE loss and the Adam optimizer.
Evaluation – performance measured with Mean Squared Error (MSE) on the test set.


Results


Final training loss: ~0.052
Test MSE: ~0.072


Skills Demonstrated


Time-series forecasting with deep learning
Sequence generation from tabular data (sliding windows)
Building and training an LSTM in PyTorch
Working with DataLoader/TensorDataset for batch training
Model evaluation using MSE
