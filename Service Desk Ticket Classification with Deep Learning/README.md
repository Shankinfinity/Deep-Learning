Overview

This project builds a deep learning model that automatically classifies customer complaints into categories (e.g. mortgage, credit card, money transfers, debt collection). It was built for CleverSupport, a company developing AI tools to improve customer support workflows.

The model is a 1D Convolutional Neural Network (CNN) built with PyTorch. It takes tokenized, padded complaint text as input, learns word embeddings, extracts local text patterns with a convolution layer, and outputs a predicted complaint category.

Workflow


Data loading – pre-tokenized words, complaint text, and labels are loaded from words.json, text.json, and labels.npy.
Preprocessing – words are mapped to integer indices, and sequences are padded/truncated to a fixed length (50 tokens).
Train/test split – 80/20 split using train_test_split.
Model – an embedding layer → 1D convolution → ReLU → global average pooling → fully connected classifier.
Training – 3 epochs using Adam optimizer and cross-entropy loss.
Evaluation – accuracy, precision, and recall (per class) computed with torchmetrics.


Results


Accuracy: ~79.6%
Precision/Recall: computed per class (5 classes), ranging roughly between 0.69–0.91


Skills Demonstrated


Natural Language Processing (tokenization, vocabulary building, padding/truncation)
Deep learning model design with PyTorch (nn.Module, nn.Embedding, nn.Conv1d)
Building custom training loops (forward pass, backpropagation, optimization)
Working with DataLoader and TensorDataset for batch training
Multi-class classification evaluation using torchmetrics (Accuracy, Precision, Recall)
End-to-end ML workflow: data preprocessing → model building → training → evaluation
