# 🧠 BPE From Scratch: Byte Pair Encoding Implementation

A complete implementation of the **Byte Pair Encoding (BPE)** algorithm built entirely from scratch using Python. This project demonstrates how subword tokenization works by learning merge rules from a custom text corpus. It also includes a simplified Transformer-inspired next-token prediction pipeline implemented with NumPy for educational purposes.

---

# 📖 Overview

Byte Pair Encoding (BPE) is one of the most widely used subword tokenization algorithms in modern Natural Language Processing (NLP). It is the foundation of tokenizers used by many Large Language Models (LLMs), including GPT, BERT, RoBERTa, and LLaMA.

This project was developed to understand the internal working of BPE without relying on external NLP libraries. Every major step of the algorithm is implemented manually, making it suitable for learning and academic demonstration.

In addition to BPE, the project includes a simple implementation of the next-token prediction pipeline using NumPy to illustrate key Transformer concepts such as embeddings, positional encoding, causal masking, self-attention, and softmax.

---

# ✨ Features

* Custom text corpus support
* Character-level tokenization
* Vocabulary creation
* Frequency-based pair counting
* Byte Pair Encoding (BPE) merge operations
* Automatic subword vocabulary generation
* Word encoding using learned merge rules
* Token decoding back to original text
* Display of learned merge rules
* Simplified Transformer-style next-token prediction
* Educational implementation using NumPy

---

# 📂 Corpus

The tokenizer is trained on a custom corpus containing words with common prefixes and suffixes.

```
low
lower
lowest
new
newer
newest
wide
wider
widest
low
lower
new
wide
```

The corpus is intentionally designed so that the BPE algorithm can efficiently learn frequently occurring subword units such as:

* low
* new
* wid
* er
* est

---

# ⚙️ Technologies Used

* Python 3
* NumPy
* collections.Counter
* Regular Expressions (re)

---

# 📁 Project Structure

```
BPE_FROM_SCRATCH/
│
├── corpus.txt
├── bpe_tokenizer.py
├── next_token_prediction.py
├── README.md
└── requirements.txt
```

---

# 🚀 Getting Started

## Clone the Repository

```bash
git clone https://github.com/keerthikamani827-jpg/BPE_FROM_SCRATCH.git
```

## Navigate to the Project

```bash
cd BPE_FROM_SCRATCH
```

## Install Required Library

```bash
pip install numpy
```

## Run the BPE Tokenizer

```bash
python bpe_tokenizer.py
```

## Run Next Token Prediction

```bash
python next_token_prediction.py
```

---

# 🔄 BPE Workflow

1. Read the input corpus.
2. Split each word into characters.
3. Build the initial vocabulary.
4. Count adjacent character pair frequencies.
5. Identify the most frequent pair.
6. Merge the pair into a new subword token.
7. Repeat the process for multiple iterations.
8. Learn merge rules.
9. Encode unseen words.
10. Decode tokens back into text.

---

# 🤖 Next Token Prediction Pipeline

The second part of the project demonstrates the fundamental stages involved in next-token prediction.

* Input Token IDs
* Embedding Layer
* Positional Encoding
* Causal Mask
* Self-Attention
* Context Vector Generation
* Linear Projection
* Softmax Probability Calculation
* Cross-Entropy Loss (Concept Demonstration)
* Next Token Prediction


---

# 📊 Sample Output

The program displays:

* Sample Corpus
* Initial Vocabulary
* Pair Frequencies
* Best Merge Pair
* Merge Operations
* Final Vocabulary
* Vocabulary Size
* Encoded Tokens
* Decoded Words
* Learned Merge Rules
* Prediction Probabilities
* Predicted Next Tokens

---

# 🎯 Learning Outcomes

After completing this project, you will understand:

* Byte Pair Encoding (BPE)
* Tokenization
* Subword Vocabulary
* Vocabulary Learning
* Encoding & Decoding
* Embedding Layer
* Positional Encoding
* Self-Attention Mechanism
* Causal Masking
* Softmax Function
* Cross-Entropy Loss
* Next Token Prediction

---

# 🔮 Future Enhancements

* Train on larger text corpora
* Save learned vocabulary to JSON
* Export merge rules
* Implement greedy decoding
* Implement beam search
* Train a complete Transformer model
* Develop a Streamlit web interface
* Visualize merge operations

---

# 👩‍💻 Author

  Keerthika M

