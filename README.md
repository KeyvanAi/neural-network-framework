# Neural Network Framework

A lightweight, modular neural network framework for deep learning and AI model development.

## Features

- **Modular Architecture** - Easily compose layers, activations, and optimizers
- **Pure Python** - No heavy dependencies, runs anywhere
- **Educational Focus** - Clean code designed for learning and experimentation
- **Extensible** - Add custom layers, loss functions, and optimizers

## Installation

```bash
git clone https://github.com/KeyvanAi/neural-network-framework.git
cd neural-network-framework
pip install -r requirements.txt
```

## Quick Start

```python
from nn_framework import NeuralNetwork, Dense, ReLU, Softmax

# Create a simple classifier
model = NeuralNetwork([
    Dense(784, 128),
    ReLU(),
    Dense(128, 10),
    Softmax()
])

# Train the model
model.fit(X_train, y_train, epochs=10, lr=0.01)

# Make predictions
predictions = model.predict(X_test)
```

## Project Structure

```
neural-network-framework/
├── nn_framework/
│   ├── __init__.py
│   ├── layers.py        # Dense, Conv2D, etc.
│   ├── activations.py   # ReLU, Sigmoid, Softmax
│   ├── optimizers.py    # SGD, Adam, RMSprop
│   └── losses.py        # CrossEntropy, MSE
├── examples/
│   ├── mnist_classifier.py
│   └── xor_example.py
├── tests/
└── README.md
```

## Supported Components

### Layers
- Dense (Fully Connected)
- Dropout
- BatchNormalization

### Activations
- ReLU, Sigmoid, Tanh, Softmax

### Optimizers
- SGD (with momentum)
- Adam
- RMSprop

### Loss Functions
- Mean Squared Error
- Cross-Entropy
- Binary Cross-Entropy

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
