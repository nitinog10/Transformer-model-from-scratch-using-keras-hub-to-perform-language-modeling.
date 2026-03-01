# Transformer-model-from-scratch-using-keras-hub-to-perform-language-modeling.
Shakespearean Transformer from Scratch with KerasHub
This repository contains a complete implementation of a Transformer model built from scratch using the keras-hub library. The model is pretrained on the Tiny Shakespeare dataset to perform causal language modeling.

Project Overview
Objective: Build and train a Transformer Decoder to generate Shakespeare-like text.
Framework: Keras 3 with the TensorFlow backend.
Key Library: keras-hub for high-level Transformer layers and preprocessing utilities.
Architecture
Tokenizer: Custom WordPieceTokenizer trained on the Shakespeare corpus (1,000 token vocabulary).
Embeddings: TokenAndPositionEmbedding with an embedding dimension of 256.
Transformer Block: TransformerDecoder with 4 attention heads and an intermediate dimension of 512.
Sequence Length: 128 tokens.
Output: Dense layer with softmax logits for vocabulary projection.
Features
Preprocessing Pipeline: Automated tokenization and shifting of sequences for causal modeling using tf.data.
Robust Inference: A custom text generation loop featuring temperature scaling and categorical sampling.
Visualization: Integrated training history plots for loss and accuracy metrics.
Results
After 10 epochs of training, the model reached:

Final Accuracy: ~28.3%
Final Loss: ~3.14
Sample Generation (Prompt: "ROMEO:"):

"romeo : that , i am not to this suffer it ; and not to me a man i did free thee..."

Requirements
pip install keras-hub keras tensorflow
