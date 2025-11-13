# 🔮 Next-Word Prediction Using a Simple RNN (PyTorch)

## 📘 Overview
This project demonstrates how to build a **Recurrent Neural Network (RNN)** from scratch using **PyTorch** to perform **next-word prediction** on a small custom text corpus.

The goal is to show how an RNN learns word dependencies and predicts the next word based on previous context — effectively creating a tiny autoregressive language model.

---

## 🚀 Features
- Builds a vocabulary from a small custom dataset.
- Converts text into sequences of `(context → next_word)` examples.
- Implements a custom `WordRNN` model using:
  - **Embedding layer**
  - **RNN layer**
  - **Fully connected prediction layer**
- Trains the model on next-word prediction.
- Includes an **autocomplete function** that generates new words based on a seed.

---

## 📂 Corpus Used
The dataset is a manually written set of short sentences:
i love to eat pizza
i love to eat pasta
i love to write code
i learn rnn
rnn is simple
rnn is cool
i like programming
programming is fun

## 🧠 Model Architecture

### **WordRNN**
| Component | Purpose |
|----------|---------|
| **Embedding Layer** | Converts word indices → dense vectors |
| **RNN Layer** | Learns sequential word dependencies |
| **Linear Layer** | Produces logits over the entire vocabulary |

---

## ⚙️ Training Configuration

| Hyperparameter | Value |
|----------------|-------|
| Embedding Size | 10 |
| Hidden Size | 32 |
| Learning Rate | 0.01 |
| Epochs | 200 |
| Optimizer | Adam |
| Loss | CrossEntropy |

