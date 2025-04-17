# Bird Species Identification Using Deep Learning

## Overview
This project applies **deep learning techniques** to identify bird species based on their vocal calls using spectrogram data derived from Xeno-Canto, a global open bird sound archive. The study involves both **binary** and **multi-class classification** using neural networks, and experiments with different model architectures and hyperparameters to maximize performance.

---

## Objectives
- Convert audio clips of bird calls into spectrograms
- Train deep learning models to identify species from these spectrograms
- Compare model accuracy across binary and multi-class setups
- Apply trained models to real-world bird call audio clips for prediction

---

## Methodology
- **Data**: Preprocessed spectrograms from 12 bird species in the Seattle region
- **Tools**: Python, Keras, TensorFlow, h5py, NumPy
- **Model Architecture**: 
  - Sequential model with Dense layers, ReLU activation, and Dropout regularization
  - Sigmoid output for binary; Softmax for multi-class
- **Training Setup**:
  - Binary classification: Black-capped Chickadee vs Blue Jay
  - Multi-class: 12 species total
  - Optimizer: RMSprop | Loss: Binary/Multi-class Cross Entropy
  - Epochs: 60 | Batch Size: 128/256
- **Performance**:
  - Binary Accuracy: **95.45%**
  - Multi-class Accuracy: **67.24%**

---

## Key Insights
| Model Type    | Best Accuracy | Notes                        |
|---------------|----------------|------------------------------|
| Binary        | 95.45%         | Blue Jay vs Chickadee       |
| Multi-class   | 67.24%         | 12 Seattle-area species     |

- Audio preprocessing (spectrogram generation) and tuning hyperparameters significantly impact performance.
- Blue Jay and Western Meadowlark calls were often confused due to similar frequency/pitch.

---

## Technologies
- Python, Keras, TensorFlow
- Spectrograms via `h5py`
- RMSprop optimizer, ReLU & Softmax activations
- Classification accuracy, confusion matrix analysis

---

## Application
- Supports biodiversity awareness and species tracking
- Potential integration into mobile wildlife/audio monitoring apps

---
