# Neural Network From Scratch (NumPy)

A complete implementation of a **Neural Network built entirely from scratch using NumPy**, implementing both **forward propagation and backpropagation without using deep learning frameworks like TensorFlow or PyTorch**.

This project demonstrates the core mathematical foundations behind neural networks, including **dense layers, activation functions, loss functions, gradient computation, and parameter updates**.

---

##  Project Overview

This project implements a fully functional neural network pipeline including:

* Forward propagation
* Backward propagation (gradient calculation)
* Softmax classification
* Categorical Cross-Entropy loss
* Accuracy evaluation
* Spiral dataset classification

The goal of this project is to **understand how neural networks work internally** by implementing every component manually.

---

##  Implemented Concepts

The following components are implemented from scratch:

### 1. Dense (Fully Connected) Layer

* Weight initialization
* Bias initialization
* Forward pass
* Backward pass (gradient calculation)

### 2. Activation Functions

* ReLU (Rectified Linear Unit)
* Softmax

### 3. Loss Function

* Categorical Cross-Entropy

### 4. Gradient Backpropagation

* Chain rule based gradient calculation
* Gradient propagation through layers

### 5. Accuracy Calculation

* Class prediction using `argmax`
* Classification accuracy evaluation

---

##  Dataset

The project uses the **Spiral Dataset**, commonly used for testing neural networks on nonlinear classification problems.

Features:

* 2 input features
* 3 classes
* 300 samples

---

##  Architecture

Neural Network Structure:

```
Input Layer (2 features)
        │
        ▼
Dense Layer (2 → 3)
        │
        ▼
ReLU Activation
        │
        ▼
Dense Layer (3 → 3)
        │
        ▼
Softmax Activation
        │
        ▼
Categorical Cross Entropy Loss
```

---

##  Forward Propagation

Forward pass computes predictions through the network:

1. Input data passes through Dense layer
2. ReLU activation introduces non-linearity
3. Second Dense layer computes class scores
4. Softmax converts scores to probabilities
5. Loss function evaluates prediction error

---

##  Backward Propagation

Backpropagation computes gradients to update weights:

1. Loss gradient is calculated
2. Softmax gradients propagate backward
3. Gradients flow through Dense layers
4. Weights and biases are updated using gradient descent

---

##  Project Structure

```
neural-network-from-scratch/
│
├── forwardpropagation.py
├── backpropagation.py

```

---

##  Key Technologies

* Python
* NumPy
* Object Oriented Programming

No external machine learning libraries are used.

---

##  Running the Project

1. Clone the repository

```bash
git clone https://github.com/yourusername/neural-network-from-scratch.git
```

2. Navigate to the project directory

```bash
cd neural-network-from-scratch
```

3. Run the script

```bash
python main.py
```

---

##  Example Output

```
Loss: 1.09
Accuracy: 0.36
```

As training progresses:

```
Loss: 0.32
Accuracy: 0.92
```

---

##  Learning Objectives

This project helps understand:

* How neural networks perform matrix computations
* How activation functions work
* How gradients are calculated
* How backpropagation trains models
* The mathematics behind deep learning

---

##  Future Improvements

* Implement Optimizers (SGD, Adam)
* Add Dropout Regularization
* Implement multiple hidden layers
* Add training loop with epochs
* Visualization of decision boundaries

---
