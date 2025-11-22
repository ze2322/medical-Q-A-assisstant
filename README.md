🏥 Medical Q&A Assistant
A fine-tuned LLaMA 3.1 8B model for answering medical questions, deployed with Streamlit.
Overview
This project uses a LoRA fine-tuned model trained on the MedQuAD dataset to provide answers to medical questions. The model is optimized for efficiency using 4-bit quantization.
⚠️ Disclaimer
This application is for educational purposes only. It is not intended to provide medical advice, diagnosis, or treatment. Always consult a qualified healthcare professional for medical concerns.
Project Structure
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
Installation

Clone the repository

bash   git clone https://github.com/yourusername/medical-qa-assistant.git
   cd medical-qa-assistant

Create a virtual environment

bash   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows

Install dependencies

bash   pip install -r requirements.txt
Usage
Run the Streamlit app:
bashstreamlit run app.py
The app will open in your browser at http://localhost:8501
Model Details

Base Model: Meta-LLaMA 3.1 8B
Fine-tuning Method: LoRA (Low-Rank Adaptation)
Training Dataset: MedQuAD
Quantization: 4-bit

LoRA Configuration

Rank (r): 8
Alpha: 8
Target Modules: q_proj, k_proj, v_proj, o_proj, gate_proj, up_proj, down_proj

Requirements

Python 3.9+
CUDA-compatible GPU (recommended: 8GB+ VRAM)
~10GB disk space for model files

License
This project is for educational purposes only.
Acknowledgments

Unsloth for efficient fine-tuning
MedQuAD dataset
Meta LLaMA for the base model
