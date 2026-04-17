# 🧠 LSTM Word Prediction

> Next-word prediction using Long Short-Term Memory (LSTM) networks — a deep learning project guided by [Campus X](https://www.youtube.com/@CampusX-official).

---

## 📌 Overview

This project implements a **word prediction model** using LSTM — a type of Recurrent Neural Network (RNN) specifically designed to learn long-range dependencies in sequential data. Given a sequence of words, the model predicts the most likely next word, mimicking the autocomplete functionality found in modern keyboards and text editors.

LSTMs solve the **vanishing gradient problem** that plagues vanilla RNNs, making them well-suited for natural language tasks.

---

## 🗂️ Project Structure

```
├── lstm_project.ipynb   # Main notebook: data prep, model, training, prediction
└── README.md
```

---

## 🔧 How It Works

The pipeline follows these key steps:

1. **Text Corpus** — A raw text dataset is loaded as the training source.
2. **Tokenization** — Words are mapped to integer indices using a vocabulary.
3. **Sequence Generation** — Fixed-length input sequences are created with a target (next word).
4. **Model Architecture** — An LSTM network is built using Keras/TensorFlow:
   - Embedding layer → encodes words as dense vectors
   - LSTM layer(s) → captures sequential context
   - Dense + Softmax output → predicts probability over vocabulary
5. **Training** — Model is trained using categorical cross-entropy loss.
6. **Prediction** — Given a seed text, the model generates the next word(s).

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core language |
| TensorFlow / Keras | Model building & training |
| NumPy | Numerical operations |
| Jupyter Notebook | Development environment |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/sanzidd/Long-Short-Term-Memory-Word-prediction-in-DL-.git
cd Long-Short-Term-Memory-Word-prediction-in-DL-
```

### 2. Install dependencies

```bash
pip install tensorflow numpy jupyter
```

### 3. Run the notebook

```bash
jupyter notebook lstm_project.ipynb
```

---

## 💡 Key Concepts

- **LSTM Gates** — Input, forget, and output gates control what information is retained or discarded across time steps.
- **Embedding Layer** — Converts sparse one-hot word representations into dense semantic vectors.
- **Sequence Length** — The window of previous words fed to the model as context.
- **Temperature Sampling** — Controls randomness in predictions (higher = more creative, lower = more conservative).

---

## 📚 Reference

This project was built as part of the **Deep Learning series by [Campus X](https://www.youtube.com/@CampusX-official)**.

---

## 📄 License

This project is open-source and available for educational use.
