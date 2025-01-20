# 🧠 Build a Generative Adversarial Network (GAN) with PyTorch  

## 🚀 Project Overview  
This project demonstrates the implementation of a **Generative Adversarial Network (GAN)** using **PyTorch**, aimed at generating synthetic data that closely resembles the original dataset. The GAN consists of two neural networks—**a Generator** and **a Discriminator**—which compete in a zero-sum game to improve the quality of generated samples over time.  

## 📊 Dataset  
The model is trained on the [MNIST dataset](http://yann.lecun.com/exdb/mnist/), a widely used benchmark for image generation tasks, consisting of grayscale handwritten digits (0-9).  

## 🏗️ Model Architecture  
The project implements:  

- **Generator:**  
  - Takes random noise as input and generates synthetic images.  
  - Utilizes transposed convolutional layers to upscale the noise.  
  - Activation functions: ReLU & Tanh for output normalization.  

- **Discriminator:**  
  - Classifies images as real or fake.  
  - A series of convolutional layers with batch normalization and LeakyReLU activation.  
  - Outputs a probability score indicating real vs. fake samples.  

## 🔧 Training Strategy  
- **Loss Function:** Binary Cross Entropy (BCE) Loss for both networks.  
- **Optimization:** Adam Optimizer with tuned learning rates.  
- **Epochs:** Configurable for improved performance.  
- **Evaluation Metrics:** Loss curves and visual comparison of generated images.  

## 📈 Results and Findings  
- Successfully generated handwritten digits resembling the original dataset.  
- The model's performance improved as training progressed, indicated by decreasing discriminator loss and stabilizing generator loss.  
- Visualizations show clear digit structures with increasing training epochs.  

## ⚡ Key Challenges  
- Balancing the training of generator and discriminator to prevent mode collapse.  
- Optimizing hyperparameters to achieve realistic output quality.  
