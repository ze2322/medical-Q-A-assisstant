# 🏥 Medical Q&A Assistant  
A fine-tuned **LLaMA 3.1 8B** model for answering medical questions, deployed with **Streamlit**.

---

## 🚀 Overview  
This project provides an AI assistant capable of answering medical questions using a **LoRA fine-tuned model** trained on the **MedQuAD** dataset.  
The model is optimized for efficient inference using **4-bit quantization**.

---

## ⚠️ Disclaimer  
This application is **for educational purposes only**.  
It is **not** intended to provide medical advice, diagnosis, or treatment.  
Always consult a qualified healthcare professional for medical concerns.

---

## 📂 Project Structure  

medical-qa-assistant/
├── medical_assistant_lora/
│ ├── adapter_config.json
│ ├── adapter_model.safetensors
│ ├── tokenizer.json
│ ├── tokenizer.model
│ ├── tokenizer_config.json
│ └── special_tokens_map.json
├── app.py
├── requirements.txt
└── README.md

---

## 📌 Requirements

Python 3.9+.
CUDA-compatible GPU (8GB+ VRAM recommended).
~10GB disk space for model + adapters.
