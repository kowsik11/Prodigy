# Task 4 - Neural Style Transfer 🎨🖌

Neural Style Transfer (NST) is a deep learning technique that blends two images — a *content image* and a *style image* — to generate a third image that preserves the content of the first while imitating the artistic style of the second.

---

## 🎯 Objective

The goal of this project is to implement and deploy a Fast Neural Style Transfer model using TensorFlow and Keras, allowing users to create unique artwork that can even be sold as NFTs.

---

## 🧠 Summary

NST uses convolutional neural networks (CNNs) to extract and recombine content and style features from different images. The loss function minimizes both:
- **Content Loss** – preserves the layout and structure.
- **Style Loss** – captures textures, colors, and patterns.

We used a pre-trained model from TensorFlow Hub:  
[Arbitrary Image Stylization v1-256](https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2)

---

## ⚙️ How to Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/deepeshdm/Neural-Style-Transfer.git
