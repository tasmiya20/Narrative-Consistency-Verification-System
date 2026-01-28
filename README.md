# Narrative-Consistency-Verification-System
## AI-Based Character Backstory Validation Using Natural Language Inference
### 📌 Overview

This project presents an AI-driven system to verify the consistency of character backstories with narrative evidence from novels.
Using Natural Language Inference (NLI) and explainable AI techniques, the system determines whether a given backstory is consistent, contradictory, or neutral with respect to the story text.

The system is designed as a multi-phase modular pipeline, making it scalable, interpretable, and suitable for low-resource narrative datasets.

### 🎯 Problem Statement

In literary analysis and storytelling systems, character backstories are often summarized manually.
However, these summaries may:

Omit key facts

Introduce inconsistencies

Contradict narrative events

This project addresses the challenge by automatically validating backstories against original narrative text, ensuring factual and contextual accuracy.

### 🧠 Key Features

📚 Automated character context extraction from novels

🔍 Evidence-based narrative retrieval

🤖 Transformer-based Natural Language Inference

🧩 Sentence-aware chunking for long texts

📊 Confidence-based decision making

🧾 Human-readable rationale generation

⚡ Fast interactive backstory verification

🏗️ System Architecture

### The system follows an 8-phase pipeline:

1. Text Ingestion – Load and preprocess raw novel text

2. Character Context Extraction – Extract evidence passages with metadata

3. Chunking Strategy – Split long text into semantic chunks

4. Feature Engineering – Enrich evidence with narrative signals

5. Model Selection – Choose optimal NLI model based on constraints

6. NLI Inference – Predict consistency between evidence and backstory

7. Rationale Generation – Generate explainable textual justifications

8. Interactive Backstory Checker – Live consistency verification

### 🧪 Models Used
Purpose	Model
Offline Evaluation	roberta-large-mnli
Fast Interactive Inference	distilroberta-base-mnli

These models are selected to balance accuracy, speed, and hardware constraints.

### 📂 Project Structure
DataDivas_KDSH_2026/
│
├── Notebooks/
│   ├── 01_Injestion.ipynb
│   ├── 02_character_context.ipynb
│   ├── 03_chunking_strategy.ipynb
│   ├── 04_feature_engineering.ipynb
│   ├── 05_model_selection.ipynb
│   ├── 06_training.ipynb
│   ├── 07_rationale_generation.ipynb
│   └── 08_inference.ipynb
│
├── phase2_output/
├── phase6_output/
├── phase7_output/
├── phase8_output/
│
├── requirements.txt
└── README.md

### 🚀 How to Run the Project
1️⃣ Create Virtual Environment
python3 -m venv jupyter_env
source jupyter_env/bin/activate

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run Phase-wise Notebooks

Execute notebooks sequentially from:

01_Injestion.ipynb → 08_inference.ipynb

### 🧾 Sample Output

Prediction Output

{
  "character": "Faria",
  "decision": "consistent",
  "confidence": 0.87,
  "supporting_evidence": "..."
}


### Rationale Output

“The evidence passage aligns with the given backstory, confirming narrative consistency with high confidence.”

### 🧠 Explainability & Trust

Unlike black-box classifiers, this system:

Grounds predictions in explicit narrative evidence

Provides human-readable rationales

Enables manual verification

This makes it suitable for research, education, and storytelling applications.

### 📚 Technologies Used

Python

Jupyter Notebook

Hugging Face Transformers

PyTorch

Pandas

Pathway (for data orchestration)

### 🏆 Applications

Literary analysis

Story summarization validation

AI-assisted writing tools

Educational platforms

Digital humanities research

