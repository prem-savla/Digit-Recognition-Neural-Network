MNIST Digit Recognition from Scratch

A neural network implementation built entirely with NumPy for handwritten digit recognition on the MNIST dataset.

This project was created as a learning exercise by studying and reproducing the ideas from an existing implementation. The goal was not to build the most accurate classifier, but to understand how neural networks work internally by implementing every major component from scratch.

The original reference that inspired this implementation is linked below.

⸻

Overview

Unlike frameworks such as TensorFlow or PyTorch, every part of the training pipeline is implemented manually using NumPy, including:

* Weight initialization
* Forward propagation
* ReLU activation
* Softmax output layer
* One-hot encoding
* Backpropagation
* Gradient descent
* Parameter updates

This project demonstrates how a simple feedforward neural network learns handwritten digit classification through iterative optimization.

⸻

Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib

⸻

Dataset

The project uses the MNIST Digit Recognizer dataset from Kaggle.

* 42,000 labeled training images
* 28 × 28 grayscale handwritten digits
* 10 output classes (0–9)

⸻

Network Architecture

Input (784 pixels)
        │
        ▼
Dense Layer (10 neurons)
        │
      ReLU
        │
        ▼
Dense Layer (10 neurons)
        │
     Softmax
        │
        ▼
Digit Prediction

⸻

Features Implemented

* Random parameter initialization
* Forward propagation
* ReLU activation
* Softmax activation
* Cross-class probability prediction
* Manual backpropagation
* Gradient descent optimization
* One-hot label encoding
* Image normalization
* Prediction visualization

⸻

Training

The network was trained using:

* Learning rate: 0.1
* Iterations: 500
* Full-batch gradient descent

Training accuracy improved steadily throughout optimization, reaching approximately 84.5%.

Validation accuracy:

* 85.4% on the held-out development set.

⸻

Example Workflow

MNIST Images
      │
Normalize Pixels
      │
      ▼
Forward Propagation
      │
      ▼
Loss Calculation
      │
      ▼
Backpropagation
      │
      ▼
Gradient Descent
      │
      ▼
Updated Parameters

⸻

Learning Objectives

This project was built to gain a deeper understanding of:

* Matrix-based neural network computation
* Gradient descent optimization
* Backpropagation mechanics
* Activation functions
* Multi-class classification
* Neural network training without deep learning libraries

Implementing these algorithms manually provides insight into the mathematical foundations behind modern machine learning frameworks.

⸻

Acknowledgements

This implementation was inspired by an existing educational tutorial. While the code was written as a hands-on replication and learning exercise, credit for the original approach belongs to the original author.

The reference implementation is linked below:

Reference: https://youtu.be/w8yWXqWQYmU?si=gVR0ke4x73NToXfN
