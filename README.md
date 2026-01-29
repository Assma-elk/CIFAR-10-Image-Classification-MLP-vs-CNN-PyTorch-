# CIFAR-10-Image-Classification-MLP-vs-CNN-PyTorch-
This project explores image classification on the CIFAR-10 dataset using two different neural network architectures: a **Multi-Layer Perceptron (MLP)** and a **Convolutional Neural Network (CNN)**. The goal is to highlight the limitations of fully connected models on image data and the benefits of convolutional inductive bias.
---

## 📊 Dataset

**CIFAR-10** is a standard computer vision dataset composed of:
- 60,000 color images (32×32)
- 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- 50,000 training images / 10,000 test images

---

## 🧠 Models

### 🔹 MLP (Baseline)
- Fully connected neural network
- Images flattened into vectors
- Used as a baseline to evaluate performance without spatial information

### 🔹 CNN
- Convolutional layers to capture spatial patterns
- Max-pooling layers for dimensionality reduction
- Data augmentation (random crops, horizontal flips)
- Weight decay and learning rate scheduling for regularization

---

## 🏋️ Training Pipeline

- PyTorch framework
- Reproducibility ensured via fixed random seeds
- Train / validation / test split
- Optimizer: Adam
- Learning rate scheduler
- Accuracy used as main evaluation metric

---

## 📈 Results (typical)

| Model | Test Accuracy |
|------|---------------|
| MLP  | ~45–50% |
| CNN  | ~70–75% |

> The CNN significantly outperforms the MLP, which is expected for image-based tasks.



## 🧩 Key Takeaways

- Fully connected networks are poorly suited for image data
- Convolutional layers effectively exploit spatial structure
- Data augmentation improves generalization
- Regularization and learning rate scheduling have a noticeable impact on performance


## 🛠 Tech Stack

- Python
- PyTorch
- NumPy
- Matplotlib


