# MNIST Handwritten Digit Classifier

A simple neural network built with TensorFlow/Keras that classifies handwritten digits (0–9) from the MNIST dataset, achieving **97–98% test accuracy**.

## 📌 Overview

This project loads the MNIST dataset using `tensorflow_datasets`, preprocesses the images (normalization, batching, shuffling, prefetching), and trains a basic fully-connected neural network to recognize handwritten digits.

## 🧠 Model Architecture

- **Input:** 28x28 grayscale images (flattened)
- **Hidden Layer:** Dense layer, 128 units, ReLU activation
- **Output Layer:** Dense layer, 10 units, Softmax activation (one per digit, 0–9)

## ⚙️ Training Details

| Setting | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Epochs | 6 |
| Batch Size | 128 |
| Test Accuracy | ~97–98% |

## 📂 Data Pipeline

- Images normalized to the [0, 1] range
- Training data shuffled and cached for performance
- Both train and test sets batched and prefetched using `tf.data.AUTOTUNE`

## 🚀 How to Run

1. Clone this repository
2. Install the required libraries:
   ```
   pip install -r requirements.txt
   ```
3. Open `mnist_model.ipynb` in Jupyter Notebook or Google Colab
4. Run all cells in order

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- TensorFlow Datasets

## 📈 Results

The model reaches approximately **97–98% accuracy** on the MNIST test set after 6 epochs of training.

## ✍️ Author

Asma Mustafa — Data Science & Machine Learning Student
- [LinkedIn](https://www.linkedin.com/in/asma-mustafa-58887b36b/)
- [GitHub](https://github.com/asmamustafa600-hub)
