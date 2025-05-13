# Deep Learning CNN TRANSFER LEARNING ON IRIS DATASET

---

## 📌 Objectives

- **CO1**: Understand the fundamentals of deep learning and convolutional neural networks.
- **CO2**: Address challenges in classification, detection, segmentation, and generation using DL architectures.
- **CO3**: Apply optimization techniques like transfer learning and hyperparameter tuning.

---

## 🧪 Part 1: Optimizers and Regularization

### ✔ Tasks

- Implemented Momentum, RMSProp, and Adam optimizers from scratch.
- Demonstrated overfitting and applied regularization: **L1**, **L2**, **Dropout**.
- Used **Iris dataset** via `load_iris()` from `sklearn`.
- Built a **Keras Sequential Model** with:
  - 3 Hidden layers (`tanh`, `tanh`, `relu`)
  - Input activation: `tanh`
  - Output activation: `softmax`
- Compared training with and without regularization.

### 🔧 Optimizers Implementation Summary

| Optimizer | Converged Iterations | Final Loss | Best Performance |
|----------:|---------------------:|-----------:|------------------|
| Momentum  | ~15                  | Moderate   | ❌               |
| RMSProp   | **7**                | ✅ Lowest  | ✅               |
| Adam      | ~10                  | Close      | ✅               |

✅ **Best Optimizer: RMSProp (Converged in 7 iterations)**

### 📉 Comparison of Optimizer
![Comparison of Optimizers](https://github.com/user-attachments/assets/6d26cedf-e789-473b-ad3c-2bfb62bb8d17)

---

## 🤖 Part 2: Transfer Learning with Pre-trained Models

### 🗃️ Datasets

- CIFAR-10
- CIFAR-100
- MNIST
- Fashion-MNIST

### 🧠 Pre-trained Models Used

- AlexNet (custom implemented)
- VGG16
- VGG19
- ResNet-50

### 🔬 Performance Comparison

| Model     | Dataset     | Accuracy | #FLOPs (Estimate) | Inference Time (s) |
|-----------|-------------|----------|-------------------|--------------------|
| VGG16     | CIFAR-10    | 64.49%   | ~15.5 GFLOPs      | 121s (5 epochs)    |
| ResNet-50 | CIFAR-10    | TBD      | TBD               | TBD                |
| AlexNet   | Fashion-MNIST | TBD    | TBD               | TBD                |

### 📊 Visualization

![Loss and Accurcy Curve](https://github.com/user-attachments/assets/615f6070-b7e3-42b1-94fc-d8beb91fa1c2)

---

## 🛠️ Requirements

- Python 3.8+
- TensorFlow / Keras
- NumPy, Pandas
- Scikit-learn
- Matplotlib / Seaborn

Install dependencies:

```bash
pip install -r requirements.txt
