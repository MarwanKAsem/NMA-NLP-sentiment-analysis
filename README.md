# NMA-NLP-sentiment-analysis

# 🧠 Tokenizer Comparison & Transfer Learning in NLP

This project explores how different tokenization strategies affect model performance in domain-specific contexts using **Twitter** and **IMDb movie review** datasets. We evaluate:
- Pre-trained tokenizers
- Custom-trained tokenizers
- Transfer learning by freezing model layers across domains

---

```
## 📂 Project Structure

.
├── data/ # Twitter and IMDb datasets
├── models/ # Saved models and tokenizers
├── notebooks/ # Jupyter notebooks for training & evaluation
├── scripts/ # Training and evaluation scripts
├── results/ # Plots and metrics
├── requirements.txt # Required Python libraries
└── README.md # Project documentation

```

---

## ⚙️ Installation

Clone the repo and install the dependencies:

```
git clone https://github.com/yourusername/tokenizer-transfer-learning.git
cd tokenizer-transfer-learning
pip install -r requirements.txt

# 🧪 Requirements

transformers==4.41.1
datasets==2.19.1
tokenizers==0.19.1
scikit-learn==1.5.0
torch==2.3.0
pandas==2.2.2
numpy==1.26.4
tqdm==4.66.4
matplotlib==3.9.0  # Optional: for visualization

```
# 🚀 Experiments
We run the following experiments:

* ✅ Baseline: Pre-trained tokenizer and model fine-tuned on Twitter (Context A)

* 🔁 Transfer Learning: Freeze model layers and apply to IMDb (Context B)

* 🛠 Custom Tokenizer: Train tokenizer on one dataset and evaluate on the other

* 📊 Evaluation: Compare accuracy across domain-matched and cross-domain scenarios

# 📈 Results
Pre-trained tokenizers perform well across domains with fine-tuning or freezing.

Domain-specific tokenizers perform better in-domain, but may degrade cross-domain.

Transfer learning is effective when tokenizer generalization is sufficient.

# Training Loss and Accuracy :
<img width="1149" height="377" alt="Training Loss And Accuracy - Copy" src="https://github.com/user-attachments/assets/24c1ea16-6c11-4a7d-a607-0bb23873dee8" />

# Transfer Learning for all Approaches :
<img width="1167" height="424" alt="Transfer learning for all Approaches" src="https://github.com/user-attachments/assets/0abee731-4fff-4e91-9d78-cf35eeb2c101" />

