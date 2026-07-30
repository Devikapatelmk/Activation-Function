
# 📘 Activation Functions Comparative Analysis using Artificial Neural Networks

## 📌 Project Overview

This project presents a comparative analysis of different activation functions used in Artificial Neural Networks (ANNs) for handwritten digit classification using the MNIST dataset.

The objective is to evaluate how different activation functions influence the learning capability and performance of a neural network while keeping the model architecture and training parameters constant.

The project was implemented using **TensorFlow/Keras** in **Google Colab**.

---

## 🎯 Objectives

- Implement common activation functions.
- Compare the behavior of activation functions.
- Study the vanishing gradient problem.
- Train ANN models using different activation functions.
- Compare model performance using various evaluation metrics.
- Identify the best activation function for the MNIST dataset.

---

## 🧠 Activation Functions Compared

- Sigmoid
- Tanh
- ReLU
- Leaky ReLU
- ELU
- Swish
- GELU

---

## 📂 Dataset

**Dataset:** MNIST Handwritten Digit Dataset

- Total Images: **70,000**
- Training Images: **60,000**
- Testing Images: **10,000**
- Number of Classes: **10**
- Image Size: **28 × 28 Pixels**

The dataset is automatically loaded using TensorFlow:

```python
from tensorflow.keras.datasets import mnist
```

---

## 🏗️ Model Architecture

The same ANN architecture was used for every activation function.

```
Input Layer (28×28)

        │

Flatten Layer

        │

Dense Layer (128 Neurons)

        │

Activation Function

        │

Dense Layer (64 Neurons)

        │

Activation Function

        │

Output Layer (10 Neurons)

        │

Softmax
```

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|--------|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Epochs | 10 |
| Batch Size | 128 |

---

## 📊 Experimental Results

| Activation Function | Test Accuracy |
|--------------------|--------------:|
| Sigmoid | 97.13% |
| Tanh | 97.51% |
| ReLU | 97.31% |
| Leaky ReLU | 97.19% |
| ELU | 97.58% |
| **Swish** | **97.80%** |
| GELU | 97.57% |

---

## 🏆 Final Model Evaluation (Swish)

| Metric | Value |
|--------|------:|
| Accuracy | **97.15%** |
| Precision | **97.22%** |
| Recall | **97.15%** |
| F1 Score | **97.16%** |

---

## 📈 Outputs

The project includes:

- Activation Function Graphs
- Derivative Graphs
- Vanishing Gradient Analysis
- Accuracy Curves
- Loss Curves
- Confusion Matrix
- Classification Report
- Performance Comparison Table

---

## 📌 Project Structure

```
Activation-Functions-ANN/
│
├── Activation_Functions.ipynb
├── README.md
├── requirements.txt
└── images/
    ├── activation_functions.png
    ├── derivatives.png
    ├── confusion_matrix.png
    ├── accuracy_curve.png
    └── loss_curve.png
```

---

## 💻 Technologies Used

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/Activation-Functions-ANN.git
```

2. Open the project folder:

```bash
cd Activation-Functions-ANN
```

3. Install the required libraries:

```bash
pip install -r requirements.txt
```

4. Open the notebook:

```
Activation_Functions.ipynb
```

5. Run all cells sequentially.

---

## 📌 Conclusion

The experimental results demonstrate that activation functions significantly influence the learning performance of Artificial Neural Networks.

Among all the evaluated activation functions, **Swish** achieved the best overall performance, producing:

- Highest Test Accuracy
- Highest Precision
- Highest Recall
- Highest F1 Score
- Smooth Gradient Flow
- Better Learning Capability

Therefore, **Swish is the most effective activation function for the MNIST handwritten digit classification task in this project.**

---

## 📚 References

1. Yann LeCun et al. — *Gradient-Based Learning Applied to Document Recognition*
2. Ramachandran, Zoph & Le — *Searching for Activation Functions*
3. TensorFlow Documentation
4. Keras Documentation
5. MNIST Handwritten Digit Dataset
