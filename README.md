# Fashion-MNIST Image Classification

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains a Convolutional Neural Network (CNN) built from scratch to classify images from the Fashion-MNIST dataset.

This project was developed as part of a Deep Learning coursework assignment. Per the assignment requirements, the model architecture is designed manually using Keras and TensorFlow. No transfer learning or pretrained models are used. The model achieves approximately 91% accuracy on the test set.

## Project Structure

```text
.
├── assets/                  # Training graphs, confusion matrix, and visual outputs
├── docs/                    # Technical report and original assignment prompt
├── logs/                    # Execution logs
├── main.py                  # Main script for data loading, training, and evaluation
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
```

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the main script to start the training process. The script handles data preprocessing, model building, training, and evaluation automatically.

```bash
python main.py
```

Running the script will output the evaluation metrics to the console and generate visual plots (accuracy/loss graphs, confusion matrix, etc.) in the `assets/` directory.

## Results

After training for 15 epochs, the model is evaluated on the independent test dataset:

*   **Test Loss**: ~0.238
*   **Test Accuracy**: ~91.4%

### Training History
The model shows stable convergence during training.
![Training Graphs](assets/training_graphs.png)

### Confusion Matrix
The confusion matrix shows the model's predictive accuracy across the 10 classes. Misclassifications are mostly between visually similar items (e.g., shirts and t-shirts).
![Confusion Matrix](assets/confusion_matrix.png)

### Predictions
Sample predictions generated on the test dataset.
![Prediction Examples](assets/prediction_examples.png)
