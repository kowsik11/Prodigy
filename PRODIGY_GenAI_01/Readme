# 🚀 GPT-2 Text Generation Model

### 👨‍💻 Author: Anurag Dhiman  
**Student | Data Scientist**

📅 **Last Updated: October 4, 2024**

---

## 📚 Overview

In recent years, the advancements in Natural Language Processing (NLP) have led to the development of powerful language models capable of generating coherent and contextually relevant text. One such model is **GPT-2**, created by **OpenAI**, widely used in applications like chatbots, story generation, and content creation.

This project demonstrates how to build a **text generation model using GPT-2**, designed for beginners with basic knowledge of Python and Machine Learning.

---

## 🔍 What is GPT-2?

**GPT-2 (Generative Pre-trained Transformer 2)** is an autoregressive language model that generates text by predicting the next word based on the previous ones. It has been trained on a massive dataset containing diverse internet text, giving it strong language understanding capabilities.

### 🔑 Key Features:
- **Text Generation**: Create coherent and grammatically correct text from a prompt.
- **Pre-trained & Fine-tunable**: Start with a powerful model and customize it with your own data.
- **Scalable**: Available in different sizes depending on your compute resources.

---

## 🧩 Project Workflow

### ✅ Step 1: Install Required Libraries

```bash
pip install transformers torch datasets gradio

### ✅ Step 2: Load GPT-2 and Tokenizer

from transformers import GPT2LMHeadModel, GPT2Tokenizer
# Load GPT-2 model and tokenizer
model_name = "gpt2"
model = GPT2LMHeadModel.from_pretrained(model_name)
tokenizer = GPT2Tokenizer.from_pretrained(model_name)

# Set to evaluation mode
model.eval()

### ✅ Step 3: Generate Text Using a Prompt

def generate_text(prompt, max_length=50):
    input_ids = tokenizer.encode(prompt, return_tensors="pt")
    output = model.generate(
        input_ids,
        max_length=max_length,
        num_return_sequences=1,
        no_repeat_ngram_size=2,
        early_stopping=True
    )
    generated_text = tokenizer.decode(output[0], skip_special_tokens=True)
    return generated_text

# Example usage
prompt = "Once upon a time"
print(generate_text(prompt, max_length=100))

✅ Sample Output
Prompt: "Once upon a time"
Generated: "Once upon a time there lived a wise old man in the hills who knew the secrets of the stars and spoke to the animals..."



