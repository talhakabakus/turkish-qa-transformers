# turkish-qa-transformers
# Exploring the Effectiveness of Pre-Trained Transformer Models for Turkish Question Answering

This repository contains the implementation of our research article titled **"Exploring the Effectiveness of Pre-Trained Transformer Models for Turkish Question Answering."** The study evaluates several pre-trained transformer architectures for their performance on a Turkish question answering (QA) benchmark dataset.

## 📄 Paper
If you use this code in your research, please cite the following paper:

> Abdullah Talha Kabakus. *Exploring the Effectiveness of Pre-Trained Transformer Models for Turkish Question Answering*. [Under Review].

## 📊 Dataset

We use the publicly available **gold-standard Turkish QA dataset** released by **Soygazi et al. (2021)**. It contains:

- **14,221** QA pairs for training  
- **3,114** QA pairs for evaluation  
- Structured in SQuAD-style JSON format

> Note: We do not host the dataset directly due to licensing. You can download it from the original [source](https://github.com/soygazisafa/TurkishQA).

## 🔍 Models Evaluated

- `electra-base-turkish-cased-discriminator`
- `XLM-RoBERTa`
- `bert-base-turkish-cased`
- `DistilBERT`
- `T5-Small`

All models were evaluated using the Hugging Face `transformers` and `datasets` libraries.

## ⚙️ Installation

```bash
git clone https://github.com/your-username/turkish-qa-transformers.git
cd turkish-qa-transformers
pip install -r requirements.txt

🚀 How to Run
	1.	Download the dataset and place it in the data/ folder.
	2.	Launch the notebook:

jupyter notebook notebooks/qa_pipeline.ipynb

	3.	Follow the steps to:
	•	Load data
	•	Preprocess using tokenizers
	•	Fine-tune transformer models
	•	Evaluate using F1 Score, Exact Match, and BLEU

📈 Evaluation Metrics

We use:
	•	F1 Score: Token-level overlap
	•	Exact Match (EM): Exact string match
	•	BLEU: N-gram-based similarity

🧪 Reproducibility

The entire workflow can be reproduced via the Jupyter notebook. Evaluation is consistent with the original dataset’s predefined train/test split.

⸻

⭐ Acknowledgments

Thanks to Soygazi et al. (2021) for providing the Turkish QA dataset.
