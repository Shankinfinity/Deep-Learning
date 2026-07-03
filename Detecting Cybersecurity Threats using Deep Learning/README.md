Overview

This project builds a deep learning model to detect malicious network activity from system logs. It uses the BETH dataset, which simulates real-world logs (process IDs, thread IDs, user IDs, etc.) with a binary label, sus_label, marking events as malicious (1) or benign (0).

Workflow


Data – load preprocessed train/test/validation logs.
Scaling – features standardized with StandardScaler.
Model – a simple feedforward neural network (Linear → ReLU → Linear → ReLU → Linear → Sigmoid) for binary classification.
Training – trained for 10 epochs using SGD optimizer and cross-entropy loss.
Evaluation – accuracy computed on train, test, and validation sets using torchmetrics.


Results


Training accuracy: ~99.97%
Validation accuracy: ~99.99%
Test accuracy: ~94.60%


Skills Demonstrated


Binary classification with deep learning
Feature scaling and preprocessing for neural networks
Building a feedforward neural network in PyTorch (nn.Sequential)
Model training and evaluation across train/val/test splits
Using torchmetrics for performance measurement
