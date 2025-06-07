🧠 AI Virtual Psychologist for Teen Mental Health

[![LLM](https://img.shields.io/badge/Model-Meta%20LLaMA%203.2-blue)]()
[![License](https://img.shields.io/badge/license-MIT-green.svg)]()
[![Made_with](https://img.shields.io/badge/Built%20With-PyTorch-orange)]()
[![Status](https://img.shields.io/badge/Status-Research--Prototype-yellow)]()

> ⚠️ *This project is a research prototype. It is not intended for real clinical use.*

💡 Overview

This repository presents a fine-tuned **Meta LLaMA 3.2 LLM** acting as a **virtual psychologist chatbot** aimed at simulating mental health support conversations, particularly for **teenagers**. The chatbot is trained using real-world-style psychiatric session transcripts and focuses on empathy, clarity, and conversational understanding.

---

🧰 Features

- 🗣️ Realistic patient–therapist conversation flow
- 🧠 Fine-tuned on structured mental health transcripts
- 🧪 Designed for interactive chat simulations
- 📊 Domain-specific emotional intelligence modeling
- 📦 Easily extendable with custom prompts or RLHF



🗂️ Repository Structure



├── Copy\_of\_Finetune\_j.ipynb      # Notebook for LLaMA 3.2 fine-tuning
├── merged\_transcripts.json       # Dataset of therapist-patient dialogues
├── requirements.txt              # Environment dependencies (optional)
└── README.md                     # Project documentation



 📁 Dataset

- **File**: `merged_transcripts.json`  
- **Format**: JSON containing `conversations` list, each with alternating `"doctor/psychologist"` and `"patient"` messages  
- **Topics Covered**: Depression, Anxiety, OCD, Mania, Suicidal ideation, Psychosis  
- **Goal**: Provide realistic training data for psychotherapy-like interactions

Link to the refernce dataset : https://github.com/nazmulkazi/dataset_automated_medical_transcription/blob/main/README.md
## 🏗️ Model & Training

- **Base Model**: Meta LLaMA 3.2
- **Platform**: Hugging Face Transformers + PyTorch
- **Finetuning Steps**:
  - Load `merged_transcripts.json`
  - Convert to instruction-prompt format
  - Tokenize using LLaMA tokenizer
  - Fine-tune using supervised learning
  - Save model checkpoint for later inference

Run locally with:

```bash
jupyter notebook Copy_of_Finetune_j.ipynb
````

> For Colab: Upload notebook + dataset, then run all cells after selecting GPU.

---

## 🚀 Quickstart

1. Clone the repo:

```bash
git clone https://github.com/yourusername/ai-virtual-psychologist.git
cd ai-virtual-psychologist
```

2. (Optional) Create environment:

```bash
pip install -r requirements.txt
```

3. Open and run the notebook:

```bash
jupyter notebook Copy_of_Finetune_j.ipynb
```

---

## 🔐 Ethics Statement

* This project does **not replace** licensed therapists or clinicians.
* Intended strictly for **educational** and **research** purposes.
* All transcripts are anonymized and simulated for safety and privacy.

---

## 🛣️ Roadmap

* [ ] Add RLHF or feedback-based improvement loop
* [ ] Deploy via API with Streamlit or Gradio interface
* [ ] Evaluate with mental health professionals
* [ ] Add safety filters for hallucination and bias detection

---

## 📢 Acknowledgements

* Meta AI for LLaMA 3.2
* Hugging Face for open-source tooling
* Open conversations & awareness around teen mental health






