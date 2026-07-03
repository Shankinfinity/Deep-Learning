Overview

This project uses a fine-tuned ResNet-18 convolutional neural network to classify chest X-rays as NORMAL or PNEUMONIA. Instead of training a CNN from scratch, it leverages a pre-trained ResNet-18 (transfer learning) to get an accurate classifier faster and with fewer resources.

Workflow


Data – 300 training and 100 test chest X-ray images (balanced across both classes), loaded with ImageFolder and DataLoader.
Preprocessing – images normalized to match ResNet-18's expected input.
Model – pre-trained ResNet-18 with frozen convolutional layers; only the final fully-connected layer is replaced and trained for binary classification.
Training – fine-tuned for 3 epochs using Adam optimizer and binary cross-entropy loss (BCEWithLogitsLoss).
Evaluation – accuracy and F1-score computed on the test set with torchmetrics, plus a visual check of predictions vs. true labels.


Results


Test accuracy: ~58%
Test F1-score: ~0.70


Skills Demonstrated


Transfer learning with a pre-trained CNN (ResNet-18)
Image preprocessing and augmentation with torchvision
Fine-tuning only the classifier head while freezing base layers
Binary image classification in PyTorch
Model evaluation with torchmetrics (Accuracy, F1-score)
Visualizing predictions with matplotlib
