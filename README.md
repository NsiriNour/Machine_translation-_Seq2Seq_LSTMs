# AI Translator: German-to-English Seq2Seq LSTM

A custom Neural Machine Translation (NMT) system built from scratch using **PyTorch**. This project implements the classic **Encoder-Decoder (Seq2Seq)** architecture to translate German sentences into English using the **Multi30K** dataset.

## 🚀 Project Overview
This project explores the foundations of NMT. It uses a "Vanilla" Seq2Seq approach where the entire meaning of a source sentence is compressed into a single **Context Vector**.

### Key Features:
- **Architecture:** Multi-layer LSTM Encoder and Decoder.
- **Data Pipeline:** Specialized IBM-style `Multi30K_de_en_dataloader.py` for text preprocessing and numericalization.
- **Inference:** Greedy Search decoding for real-time translation.

## 📊 Training Results
Trained for 15 epochs on a CPU. Despite the lack of an attention mechanism, the model achieved significant convergence:
- **Initial Loss:** 5.29
- **Final Loss:** ~2.70
- **Final Perplexity (PPL):** Successfully dropped from 198 to below 20.

### The Learning Curve
<img width="1016" height="614" alt="image" src="https://github.com/user-attachments/assets/396b01cc-e553-4af1-8497-197078392cc1" />

*The smooth downward trend proves that the LSTM successfully learned to map German syntax to English semantics.*

## 🛠️ Tech Stack
- **Framework:** PyTorch (nn, optim, functional)
- **NLP:** SpaCy, NLTK
- **Development:** Python 3.12, Miniconda

## 🧠 Future Work
- **Attention Mechanism:** Implementing a Bahdanau Attention layer to improve performance on longer sentences.
- **Transformers**
