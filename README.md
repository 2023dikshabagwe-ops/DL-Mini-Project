# DL-Mini-Project
# CycleGAN-Based Image Translation using Deep Learning

## 📌 Project Overview

This project implements a **CycleGAN (Cycle Generative Adversarial Network)** model for **image-to-image translation** using **PyTorch**.  
The notebook demonstrates the complete workflow of building, training, and evaluating a deep learning model capable of translating images from one domain to another without requiring paired training data.

The project includes:

- Image preprocessing and augmentation
- Custom dataset creation
- Generator and Discriminator models
- Cycle consistency loss implementation
- Identity loss
- Perceptual loss using VGG19
- Gaussian blur enhancement
- Training pipeline
- Image visualization and testing

The entire implementation is provided in the Jupyter Notebook:

```text
DL_Miniproject.ipynb
```

---

# 🎯 Objectives

The main objectives of this project are:

- To understand the architecture and working of CycleGANs
- To implement image-to-image translation using deep learning
- To train adversarial neural networks using PyTorch
- To apply perceptual and cycle consistency losses
- To visualize generated outputs and evaluate performance

---

# 🧠 About CycleGAN

CycleGAN is a type of **Generative Adversarial Network (GAN)** used for unpaired image translation tasks.

Unlike traditional GANs, CycleGAN does not require paired datasets.  
It learns mappings between two image domains using:

- Two Generators
- Two Discriminators
- Cycle Consistency Loss

Examples of applications include:

- Horse ↔ Zebra translation
- Summer ↔ Winter conversion
- Monet painting style transfer
- Black & white ↔ Color image generation

---

# 🛠️ Technologies and Libraries Used

## Programming Language

- Python 3.x

## Deep Learning Framework

- PyTorch

## Libraries Used

- torchvision
- numpy
- matplotlib
- PIL (Python Imaging Library)
- torch.nn
- torch.optim

---

# 📂 Project Structure

```text
Deep-Learning-MiniProject/
│
├── DL_Miniproject.ipynb
├── README.md
├── dataset/
│   ├── trainA/
│   ├── trainB/
│   ├── testA/
│   └── testB/
│
└── outputs/
    ├── generated_images/
    └── training_results/
```

---

# ⚙️ Features Implemented

## ✅ Custom Dataset Loader

- Loads images from folders
- Applies preprocessing and transformations
- Converts images into tensors for training

---

## ✅ Image Preprocessing

Includes:

- Resizing
- Normalization
- Tensor conversion
- Data augmentation

---

## ✅ Generator Network

The generator learns to translate images between domains.

Features:
- Convolution layers
- Residual blocks
- Activation functions
- Upsampling layers

---

## ✅ Discriminator Network

The discriminator distinguishes:
- Real images
- Generated images

Used for adversarial training.

---

## ✅ Cycle Consistency Loss

Ensures that:
- Image translated from Domain A → B
- and back from B → A

remains similar to the original image.

---

## ✅ Identity Loss

Helps preserve:
- Color composition
- Structural details

during translation.

---

## ✅ Perceptual Loss using VGG19

Improves visual quality by comparing:
- High-level feature representations
instead of only pixel values.

---

## ✅ Gaussian Blur Enhancement

Post-processing technique used to:
- Smooth generated images
- Improve visual appearance

---

## ✅ Training Visualization

The notebook visualizes:
- Generated outputs
- Loss curves
- Intermediate training results

using Matplotlib.

---

# 🧮 Model Architecture

## Generator Architecture

The Generator consists of:

1. Initial convolution layer
2. Downsampling layers
3. Residual blocks
4. Upsampling layers
5. Output convolution layer

---

## Discriminator Architecture

PatchGAN discriminator is used to:
- Classify image patches
instead of the full image.

This improves:
- Training stability
- Texture generation quality

---

# 🔄 Training Workflow

The training process follows these steps:

1. Load images from both domains
2. Preprocess and normalize images
3. Generate translated images
4. Compute adversarial loss
5. Compute cycle consistency loss
6. Compute identity loss
7. Backpropagation and optimization
8. Save generated outputs

---

# 📊 Loss Functions Used

## Adversarial Loss

Used to train:
- Generator
- Discriminator

through adversarial learning.

---

## Cycle Consistency Loss

Ensures reconstructed images remain close to original images.

---

## Identity Loss

Maintains:
- Color consistency
- Structural integrity

---

## Perceptual Loss

Uses pretrained VGG19 features for:
- Better visual quality
- Enhanced texture learning

---

# 📈 Results

The project successfully demonstrates:

- Image-to-image translation
- Stable adversarial training
- Visual output generation
- Improved image quality using perceptual loss

Generated outputs are visualized directly in the notebook.

---

# 🚀 Installation

Install required dependencies:

```bash
pip install torch torchvision matplotlib numpy pillow
```

---

# ▶️ How to Run the Project

## Step 1: Clone Repository

```bash
git clone <repository-link>
```

---

## Step 2: Open Project Folder

```bash
cd Deep-Learning-MiniProject
```

---

## Step 3: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
DL_Miniproject.ipynb
```

---

## Step 4: Run All Cells

Execute the notebook sequentially.

---

# 💻 Hardware Requirements

Recommended:

- GPU (CUDA-enabled)
- Minimum 8 GB RAM
- Python 3.9+

---

# 📚 Concepts Covered

This project demonstrates practical implementation of:

- Deep Learning
- Computer Vision
- GANs
- CycleGAN
- Image Processing
- Transfer Learning
- Perceptual Loss
- PyTorch Training Pipelines

---

# 🔍 Applications of CycleGAN

CycleGAN can be applied in:

- Artistic style transfer
- Medical image translation
- Image enhancement
- Weather conversion
- Day-to-night transformation
- Photo generation

---

# 📌 Future Improvements

Possible future enhancements:

- Add FID score evaluation
- Use larger datasets
- Implement attention mechanisms
- Deploy using Streamlit or Flask
- Add model checkpoint saving
- Improve training efficiency

---


# 📄 License

This project is created for educational and academic purposes.
