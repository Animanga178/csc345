<h1 align="center">
    CIFAR-100 Image Classification with Deep Learning
</h1>

<h4 align="center">A comparative study of fully connected and convolutional neural networks on fine and coarse image classification using the CIFAR-100 dataset.</h4>

<p align="center">
  <a href="#project-overview">Project Overview</a> •
  <a href="#methodology">Methodology</a> •
  <a href="#results">Results</a> •
  <a href="#how-to-use">How to Use</a> •
  <a href="#credits">Credits</a> •
  <a href="#license">License</a>
</p>

---

## 🧠 Project Overview

This project was submitted as part of the CSC345: Big Data and Machine Learning module and received a grade of **84%**.

The objective was to investigate and compare the performance of two deep learning models— a fully connected neural network (NN) and a convolutional neural network (CNN)—on the CIFAR-100 dataset, using both fine-grained (100-class) and coarse-grained (20-class) classification labels.

---

## 🔬 Methodology

Two models were developed and evaluated:

### 1. Fully Connected Neural Network (NN)
- Input: Flattened 32×32×3 images
- Architecture: Two dense layers (256 → 128), ReLU activation, HeNormal initialisation
- Regularisation: Dropout (0.3)
- Optimiser: Adam
- Output: Softmax over 100/20 classes

### 2. Convolutional Neural Network (CNN)
- Two convolutional blocks with 64 and 128 filters
- ReLU activations, max pooling, dropout (0.5)
- Dense layer for final classification
- Optimised with Adam and early stopping

Both models were trained for up to 20 epochs and evaluated on classification accuracy.

---

## 📈 Results

| Task            | Benchmark | Fully Connected NN | CNN          |
|-----------------|-----------|--------------------|--------------|
| Fine-Grained    | 24.49%    | 21.6%              | **32.9%**    |
| Coarse-Grained  | 39.43%    | 33.7%              | **47.3%**    |

- The CNN significantly outperformed the NN on both tasks.
- Better performance was observed in coarse-grained classification for both models.

> These results reinforce the effectiveness of CNNs in visual tasks and highlight the limits of basic dense architectures in complex datasets like CIFAR-100.

---

## 🛠 How to Use

1. **Clone this repository**
   ```bash
   git clone https://github.com/Animanga178/csc345.git
   cd csc345

## 📚 Credits

- Dataset: CIFAR-100
- Fully connected and CNN architectures implemented using TensorFlow/Keras or PyTorch
- Performance benchmark based on CIFAR-100 baselines
- Report written by Alicia Addo (2024) for CSC345: Big Data and Machine Learning

  
