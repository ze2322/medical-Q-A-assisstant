## 🏥 Medical Q&A Assistant

A fine-tuned LLaMA 3.1 8B model for answering medical questions, deployed with Streamlit.

## 🚀 Overview

This project provides an AI assistant capable of answering medical questions using a LoRA fine-tuned model trained on the MedQuAD dataset.
The model is optimized for efficient inference using 4-bit quantization.

## ⚠️ Disclaimer

This application is for educational purposes only.
It is not intended to provide medical advice, diagnosis, or treatment.
Always consult a qualified healthcare professional for medical concerns.

## 📂 Project Structure
medical-qa-assistant/
├── medical_assistant_lora/
│   ├── adapter_config.json
│   ├── adapter_model.safetensors
│   ├── tokenizer.json
│   ├── tokenizer.model
│   ├── tokenizer_config.json
│   └── special_tokens_map.json
├── app.py
├── requirements.txt
└── README.md

## 📌 Requirements

Python 3.9+

CUDA-compatible GPU (8GB+ VRAM recommended)

~10GB disk space for model + adapters

## 🛠 Installation

# 1️⃣ Clone the repository
git clone https://github.com/yourusername/medical-qa-assistant.git
cd medical-qa-assistant

# 2️⃣ Create a virtual environment
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

▶️ Usage

Run the Streamlit app:

streamlit run app.py


The app will open at:
http://localhost:8501

🧠 Model Details

Base Model: Meta LLaMA 3.1 8B

Fine-tuning Method: LoRA

Training Dataset: MedQuAD

Quantization: 4-bit

🔧 LoRA Configuration

Rank (r): 8

Alpha: 8

Target Modules: q_proj, k_proj, v_proj, o_proj, gate_proj, up_proj, down_proj

📄 License

This project is for educational purposes only.

🙏 Acknowledgments

Unsloth – efficient LoRA fine-tuning

MedQuAD dataset

Meta LLaMA – base model
