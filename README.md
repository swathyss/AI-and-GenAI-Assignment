# 🎨 MNIST Digit Generation using GAN (Generative Adversarial Network)

![Python](https://img.shields.io/badge/Python-3.9-blue)  
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)  
![GAN](https://img.shields.io/badge/Model-GAN-green)  
![Dataset](https://img.shields.io/badge/Dataset-MNIST-yellow)

A deep learning project focused on building and training a **Generative Adversarial Network (GAN)** to generate realistic handwritten digit images similar to the **MNIST dataset**.

---

# 📘 Project Overview

This project implements a **GAN architecture** consisting of a **Generator** and a **Discriminator** that compete against each other to produce realistic images.

The project covers:

- Loading and preprocessing MNIST dataset  
- Designing Generator and Discriminator networks  
- Training adversarial models  
- Monitoring loss functions  
- Visualizing generated images  

The goal is to generate **high-quality handwritten digit images from random noise**.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Understand Generative Adversarial Networks (GANs)  
🔹 Build Generator and Discriminator models  
🔹 Train models using adversarial learning  
🔹 Generate realistic handwritten digits  
🔹 Analyze training stability and performance  

---

# 📂 Dataset Information

The dataset used is the **MNIST Handwritten Digits Dataset**.

### Dataset Details

| Feature | Description |
|--------|------------|
| Image Size | 28 × 28 pixels |
| Channels | Grayscale (1 channel) |
| Classes | Digits (0–9) |
| Training Samples | 60,000 |
| Test Samples | 10,000 |

---

# 🧹 Data Preprocessing

Before training the model, the following steps were applied:

### ✔ Normalization
- Pixel values scaled to range **[-1, 1]**

### ✔ Reshaping
- Images reshaped to **(28, 28, 1)**

---

# 🧠 GAN Architecture

The GAN consists of two neural networks:

---

## 🔹 Generator

- Input: Random noise vector (e.g., 100 dimensions)  
- Output: 28×28 grayscale image  

### Layers:
- Dense  
- BatchNormalization  
- LeakyReLU  
- Conv2DTranspose  
- Output Layer (Tanh activation)  

---

## 🔹 Discriminator

- Input: Real or generated image  
- Output: Probability (Real = 1, Fake = 0)  

### Layers:
- Conv2D  
- LeakyReLU  
- Dropout  
- Flatten  
- Dense (Sigmoid activation)  

---

# ⚙️ Model Training

### Training Configuration

- Loss Function: Binary Cross-Entropy (BCE)  
- Optimizer: Adam  
- Learning Rate: 0.0002  
- Beta1: 0.5  
- Epochs: 20+  

---

# 📊 Training Monitoring

During training:

- Generator loss and Discriminator loss are tracked  
- Model performance improves over epochs  
- Stability between networks is analyzed  

---

# 🔍 Output Visualization

To evaluate results:

- Generated images displayed in grid format  
- Visual comparison with real MNIST digits  
- Progress observed across epochs  

---

# 🛠 Tech Stack

| Tool | Purpose |
|----|--------|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Google Colab / Jupyter | Development environment |

---

# 📁 Repository Structure

gan-mnist-project/

│  
├── AI_and_GenAI_Assignment.ipynb  
├── AI and GenAI Assignment.pdf  
└── README.md  

---

# 🚀 How to Run the Project

### 1️⃣ Install Dependencies

pip install tensorflow numpy matplotlib

---

### 2️⃣ Run the Notebook

- Open the `.ipynb` file in Jupyter Notebook or Google Colab  
- Run all cells sequentially  

---

### 3️⃣ Model Workflow

- Load MNIST dataset  
- Preprocess data  
- Build Generator & Discriminator  
- Train GAN model  
- Visualize generated images  

---

# 📈 Results

- GAN successfully generates handwritten digits  
- Image quality improves with training epochs  
- Loss curves indicate adversarial learning behavior  

---

# 🧠 Key Learning Outcomes

✔ Understanding GAN architecture  
✔ Adversarial training concepts  
✔ Image generation using deep learning  
✔ Training instability challenges in GANs  
✔ Visualization of generated outputs  

---

# 📌 Academic Submission

This project was developed as part of an **AI & Generative AI assignment** to demonstrate the implementation of a **Generative Adversarial Network (GAN) for handwritten digit generation using the MNIST dataset**.
