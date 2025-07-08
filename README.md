# 🧠 Handwritten Digit Recognition with MNIST & Neural Networks

This project uses a deep learning model built with **TensorFlow and Keras** to classify handwritten digits from the **MNIST dataset**. It also includes a custom prediction system that accepts an external image and predicts the digit.

> 🔗 Inspired by classic computer vision tasks and ideal for beginners in deep learning.

---

## 📌 Demo

![MNIST Sample](https://upload.wikimedia.org/wikipedia/commons/2/27/MnistExamples.png)

---

## 📂 Dataset Used

**MNIST Dataset**  
- 🖼️ 28x28 grayscale images  
- 🔢 Labels: 0–9  
- 🧪 60,000 training samples  
- 🧾 10,000 test samples  
- Preloaded in Keras: `from keras.datasets import mnist`

---

## 🚀 Features

- Load and explore MNIST data
- Normalize and preprocess data
- Train a deep neural network
- Evaluate accuracy and loss
- Generate predictions and labels
- Visualize confusion matrix
- Accept an external image and predict its digit using OpenCV

---

## 🛠️ Tech Stack

| Tool         | Purpose                         |
|--------------|----------------------------------|
| Python       | Programming Language             |
| NumPy        | Numerical operations             |
| Matplotlib   | Image visualization              |
| Seaborn      | Confusion matrix visualization   |
| OpenCV       | Preprocessing external images    |
| TensorFlow/Keras | Building & training the model |

---

## 🧪 Model Architecture

- `Flatten` Layer → Converts 28x28 to 784 vector
- `Dense (50, relu)`
- `Dense (50, relu)`
- `Dense (10, sigmoid)` → For 10 digit classes

> Loss: `sparse_categorical_crossentropy`  
> Optimizer: `adam`  
> Epochs: `10`

---

## 📊 Results

- Model trained for 10 epochs
- Test accuracy typically around **97–98%**
- Supports external digit image classification (28x28 grayscale JPEG)

---

## 🧩 Confusion Matrix

Used to visualize model performance across different digits:
```python
confusion_matrix(y_true, y_pred)
sns.heatmap(..., annot=True)
