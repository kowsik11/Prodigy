# 🎨 Task 2: Text-to-Image Generation using Pretrained Models

**🔬 Project Title:** Generating Images from Text Prompts using DALL·E Mini and Stable Diffusion  
**👨‍💻 Author:** Anurag Dhiman  
📅 **Date:** October 6, 2024  

---

## 📌 Table of Contents
1. [Overview](#overview)
2. [Technologies Used](#technologies-used)
3. [Setup & Installation](#setup--installation)
4. [Using DALL·E Mini](#using-dall·e-mini)
5. [Using Stable Diffusion](#using-stable-diffusion)
6. [Sample Outputs](#sample-outputs)
7. [Use Cases](#use-cases)
8. [Future Improvements](#future-improvements)
9. [Contact](#contact)

---

## 📚 Overview

This task focuses on generating visually compelling images from simple **text prompts** using powerful **pretrained generative models** like **DALL·E Mini** and **Stable Diffusion**.

These models transform natural language descriptions into synthetic, realistic images — enabling AI to visualize your imagination.

---

## 🛠️ Technologies Used

| Tool/Library       | Description                                 |
|--------------------|---------------------------------------------|
| `transformers`     | For working with pretrained models          |
| `diffusers`        | For Stable Diffusion pipelines              |
| `DALL·E Mini` / `Craiyon` | Lightweight image generation from text |
| `torch`, `numpy`   | Core ML and tensor ops                      |
| `PIL`              | Image display and saving                    |
| `gradio` (optional)| UI for real-time prompting                  |

---

## ⚙️ Setup & Installation

### ✅ Install Required Libraries

```bash
pip install torch torchvision diffusers transformers pillow gradio


🎨 Using Stable Diffusion (Python Code)
python
Copy
Edit
from diffusers import StableDiffusionPipeline
import torch

# Load Stable Diffusion
pipe = StableDiffusionPipeline.from_pretrained("CompVis/stable-diffusion-v1-4", torch_dtype=torch.float16)
pipe = pipe.to("cuda")

# Define a text prompt
prompt = "A steampunk airship flying above the clouds during sunset"

# Generate image
image = pipe(prompt).images[0]

# Save image
image.save("steampunk_airship.png")

# Display (if in notebook)
image.show()
📌 Note: You need a CUDA-compatible GPU for best performance.


---

✅ You can now copy this **entire README file** into your GitHub project under **Task 2 folder**.

Would you like me to generate a sample `.py` file (`text_to_image.py`) for Stable Diffusion as well?
