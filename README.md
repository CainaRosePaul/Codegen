# CodeGen LLM Fine-Tuning for Python Code Generation

This project explores fine-tuning the **Salesforce CodeGen large language model** for Python code generation using **parameter-efficient fine-tuning (LoRA/PEFT)**.

## Problem
Pretrained code generation models often produce incomplete or incorrect outputs when given natural language instructions.  
The goal of this project was to improve the quality of generated Python code by fine-tuning CodeGen on curated instruction–code datasets.

## Approach
The project implements an end-to-end LLM experimentation pipeline:

1. Dataset preparation and formatting for instruction–code pairs
2. Model loading with **4-bit quantization (BitsAndBytes)** for efficient training
3. Parameter-efficient fine-tuning using **LoRA (PEFT)**
4. Evaluation using **CodeBLEU metrics**
5. Comparison of multiple fine-tuning strategies
6. Deployment of an interactive demo using **Streamlit**

## Technologies
- Python
- Hugging Face Transformers
- PEFT / LoRA
- BitsAndBytes quantization
- CodeBLEU evaluation
- Streamlit (for demo interface)

## Results
Fine-tuning improved the **CodeBLEU score by ~8%**, demonstrating better code structure and semantic correctness in generated outputs.

## Repository Contents
- `Codegen_fine_tuning_Code.ipynb` – training and evaluation pipeline
- dataset preprocessing and evaluation scripts
- visualization of CodeBLEU performance across models

## Future Work
- integrate retrieval-augmented code generation
- expand dataset size for improved generalization
- deploy as an API-based inference service

---

Author: Caina Rose Paul
