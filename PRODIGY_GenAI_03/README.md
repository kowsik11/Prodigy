# Task 3 - Image-to-Image Translation using Conditional GANs (pix2pix)

This project implements image-to-image translation using Conditional Adversarial Networks, based on the [pix2pix paper](https://phillipi.github.io/pix2pix/) by Phillip Isola *et al*.

---

## 📌 Project Overview

This task explores converting one image domain into another (e.g., edges to objects, maps to satellite views) using a conditional GAN approach. It leverages:
- A **U-Net Generator** (encoder-decoder with skip connections)
- A **PatchGAN Discriminator** (for local-level realism)

---

## 📁 Datasets Used

- Facades  
- Maps (Map-to-Satellite and Satellite-to-Map)

Datasets are sourced from the official [pix2pix dataset collection](http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/).

---

## ⚙️ Prerequisites

- Python 3.7+
- PyTorch 1.0+  
- CUDA (optional for GPU training)

---

## 🚀 Getting Started

1. Clone the repo and navigate to the project directory  
2. Install dependencies  
3. Train the model:
   ```bash
   python src/main.py --mode train --data_root '../datasets/maps' --num_epochs 100 --data_invert
