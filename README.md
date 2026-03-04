# Outfit Generation with Stable Diffusion LoRA

This project explores **fine-tuning Stable Diffusion v1.5 using Low-Rank Adaptation (LoRA)** for generating fashion outfits from text prompts.

The objective is to specialize a general text-to-image diffusion model to generate **fashion-related outfits** using a curated dataset of clothing products.

The project includes the full pipeline from training to inference and provides an interactive interface for testing the model.

---

# Project Highlights

• Fine-tuning **Stable Diffusion v1.5** with **LoRA adapters**

• Training performed on a **fashion product dataset with captions**

• Comparison between:
  - Baseline Stable Diffusion
  - Fine-tuned LoRA model

• Implementation using the **Diffusers library**

• Experiment tracking using **Weights & Biases (W&B)**

• Interactive **Gradio interface** for real-time image generation

• Reproducible pipeline for training and inference

---

---

# Model Training

The LoRA model is trained on the dataset:
hahminlew/kream-product-blip-captions


Key training configuration:

| Parameter | Value |
|--------|------|
| Base model | Stable Diffusion v1.5 |
| Resolution | 512 |
| Learning rate | 1e-4 |
| Train steps | 2000 |
| Gradient accumulation | 4 |
| LoRA rank | 64 |
| Mixed precision | fp16 |

---

