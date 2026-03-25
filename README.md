# 🧠 Domain-Specific LLM Fine-Tuning using TinyLlama + LoRA

## 📌 Overview
This project demonstrates domain-specific fine-tuning of a pretrained Large Language Model (LLM) using non-instructional data. The model is adapted to a specialized domain (medical/pharmaceutical) by extracting text from PDF documents and training using parameter-efficient techniques.

---

## 🚀 Features
- 📄 Extracts domain-specific data from PDF documents  
- 🔤 Tokenizes and preprocesses custom dataset  
- 🤖 Fine-tunes pretrained LLM (TinyLlama 1.1B)  
- ⚡ Uses LoRA (Low-Rank Adaptation) for efficient training  
- 💾 Applies 8-bit quantization (BitsAndBytes) for memory optimization  
- 🔁 End-to-end pipeline from data extraction → training → inference  

---

## 🏗️ Tech Stack
- Python  
- Hugging Face Transformers  
- Hugging Face Datasets  
- PEFT (LoRA)  
- BitsAndBytes (8-bit quantization)  
- PyMuPDF (PDF text extraction)  
- Google Colab  

---

## 📂 Project Structure
```text
├── data/
│   └── extracted_text.txt
├── notebooks/
│   └── finetuning.ipynb
├── models/
│   └── fine_tuned_model/
└── README.md
```


## ⚙️ Workflow
1. Data Extraction
- Extract text from domain-specific PDF using PyMuPDF
- Clean and structure text for training

2. Dataset Preparation
- Convert extracted text into training dataset
- Tokenize using Hugging Face tokenizer

3. Model Loading
- Load pretrained TinyLlama 1.1B model
- Enable 8-bit quantization for efficiency

4. Fine-Tuning
- Apply LoRA (Low-Rank Adaptation)
- Train model on domain-specific dataset

5. Inference
- Generate domain-aware responses using fine-tuned model

## 🧪 Example Use Case

Input:

What is Metformin used for?

Output (after fine-tuning):

Metformin is commonly used to manage type 2 diabetes by improving insulin sensitivity and reducing glucose production in the liver.


## 📊 Key Highlights
- Efficient fine-tuning using LoRA reduces computational cost

- 8-bit quantization enables training on limited hardware

- Domain adaptation improves contextual accuracy

- Real-world dataset (PDF-based) used instead of synthetic data

## 📦 Installation
```text Bash 
pip install transformers datasets peft bitsandbytes pymupdf accelerate
```
▶️ Usage

- Open the notebook in Google Colab

- Upload your domain-specific PDF

- Run all cells step-by-step

- Fine-tune the model

- Test with custom prompts

## 🔮 Future Improvements

- [ ] Add evaluation metrics (BLEU, ROUGE)

- [ ] Build a UI using Streamlit

- [ ] Deploy as an API using FastAPI

- [ ] Compare base vs fine-tuned model outputs


## 🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit pull requests.


## 📜 License
This project is open-source and available under the MIT License.

## 👨‍💻 Author
Venkatesh Pamudurti

GitHub: [@Venkat5674](https://github.com/Venkat5674/)

LinkedIn: [Venkatesh Pamudurti](https://www.linkedin.com/in/venkatesh-pamudurti/)

## ⭐ Support
If you found this project helpful, please give it a ⭐ on GitHub!
