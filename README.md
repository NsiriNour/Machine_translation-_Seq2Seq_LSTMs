# 🌍 AI Translator: German-to-English Seq2Seq with Attention

An end-to-end Neural Machine Translation (NMT) system built from scratch using PyTorch. This project implements a Sequence-to-Sequence (Seq2Seq) architecture optimized with an **Attention Mechanism** to translate German sentences into English.

## 🚀 Features
- **Encoder-Decoder Architecture:** Built using LSTMs/GRUs.
- **Attention Mechanism:** Implemented a Bahdanau-style attention to handle long-range dependencies and improve translation accuracy.
- **Custom Data Pipeline:** Modern implementation using Hugging Face `datasets` and `SpaCy` tokenizers, bypassing deprecated `torchtext` utilities.
- **Interactive UI:** A fully functional web interface built with **Gradio** for real-time testing.
- **Performance Metrics:** Evaluated using **BLEU Score** and **Perplexity**.

## 📊 Performance
- **Dataset:** Multi30K (German-English)
- **Training:** 20 Epochs on CPU/GPU
- **Best BLEU Score:** [INSERT YOUR SCORE HERE, e.g., 28.50]
- **Key Metric:** Successfully eliminated word repetition and "forgetting" through the Attention layer.

### Loss Curve
![Loss Graph]([INSERT_LINK_TO_YOUR_GRAPH_IMAGE_HERE])
*The graph shows a healthy convergence between Training and Validation loss, indicating effective generalization.*

## 🛠️ Tech Stack
- **Framework:** PyTorch
- **Data:** Hugging Face `datasets`
- **NLP:** SpaCy, NLTK (BLEU)
- **Interface:** Gradio
- **Development:** Python, Jupyter Notebook

## 💻 Installation & Usage
1. Clone the repo:
   ```bash
   git clone https://github.com/[YOUR_USERNAME]/ai-translator-lstm.git
