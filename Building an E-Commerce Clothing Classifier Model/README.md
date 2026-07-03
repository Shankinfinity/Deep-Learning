This project builds a Convolutional Neural Network (CNN) to automatically classify clothing images into garment types (shirts, trousers, shoes, etc.). It was built for Fashion Forward, an AI-based e-commerce retailer, to automate product tagging and improve inventory management.

Workflow


Data – the FashionMNIST dataset (10 clothing categories) loaded via torchvision.datasets.
Model – a custom CNN (ClothingCNN) with 2 convolutional layers, max pooling, and 2 fully connected layers.
Training – trained for 1 epoch using Adam optimizer and cross-entropy loss.
Evaluation – accuracy, and per-class precision and recall computed with torchmetrics.
Visualization – sample test predictions plotted against true labels.


Results


Accuracy: ~86.7%
Precision/Recall (per class): ranging roughly between 0.64–0.98


Skills Demonstrated


Image classification with Convolutional Neural Networks (CNNs)
Building a custom CNN architecture in PyTorch
Working with DataLoader for image batching
Multi-class evaluation using torchmetrics (Accuracy, Precision, Recall)
Visualizing model predictions with matplotlib
