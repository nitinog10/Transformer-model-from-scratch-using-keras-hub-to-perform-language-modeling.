# Shakespearean Transformer from Scratch with KerasHub

A complete implementation of a Transformer **Decoder** built from scratch using **keras-hub** and **Keras 3** (TensorFlow backend). The model is pretrained on the **Tiny Shakespeare** dataset for **causal language modeling** and generates Shakespeare-like text.

---

## ✨ Project Overview

**Objective:** Build and train a Transformer Decoder to generate Shakespeare-style text  
**Framework:** Keras 3 with the TensorFlow backend  
**Key Library:** `keras-hub` for high-level Transformer layers and preprocessing utilities

---

## 🧠 Architecture

- **Tokenizer:** Custom `WordPieceTokenizer` trained on the Shakespeare corpus (1,000 token vocabulary)
- **Embeddings:** `TokenAndPositionEmbedding` with embedding dimension **256**
- **Transformer Block:** `TransformerDecoder` with **4 attention heads** and intermediate dimension **512**
- **Sequence Length:** **128 tokens**
- **Output:** Dense layer with softmax logits for vocabulary projection

---

## ✅ Features

- **Preprocessing Pipeline:** Automated tokenization and shifting of sequences for causal modeling using `tf.data`
- **Robust Inference:** Custom text generation loop with **temperature scaling** and **categorical sampling**
- **Visualization:** Training history plots for loss and accuracy metrics

---

## 📈 Results

After **10 epochs** of training:

- **Final Accuracy:** ~28.3%
- **Final Loss:** ~3.14

**Sample Generation (Prompt: "ROMEO:")**  
> "romeo : that , i am not to this suffer it ; and not to me a man i did free thee..."

---

## 📦 Requirements

```bash
pip install keras-hub keras tensorflow
```

---

## 🚀 Usage

1. Prepare the Tiny Shakespeare dataset.
2. Train the WordPiece tokenizer.
3. Train the Transformer Decoder model.
4. Generate text using the inference loop.

> (Include your training/inference script usage here if available.)

---

## 📝 Notes

This project is designed to demonstrate:
- Transformer decoders from first principles
- End-to-end preprocessing in Keras 3
- Text generation with controllable randomness

---

## 🙌 Acknowledgements

- [keras-hub](https://keras.io/keras_hub/)
- Tiny Shakespeare dataset
