# gpt-from-scratch
GPT From Scratch

Recreating and learning the inner workings of a Generative Pretrained Transformer (GPT) by following Andrej Karpathy’s tutorial:
Let’s build GPT: from scratch, in code, spelled out

This project is a hands-on implementation of a GPT-style language model using PyTorch, built step-by-step to better understand how modern large language models actually work under the hood. Inspired by OpenAI’s GPT-2 architecture and the original Attention Is All You Need transformer paper, this repository focuses on learning by building everything from first principles.

Project Goals
Understand transformer architecture from the ground up
Implement self-attention and multi-head attention manually
Train a character-level language model
Explore tokenization, embeddings, positional encoding, and autoregressive generation
Learn the training pipeline behind modern LLMs
Gain deeper intuition for how GPT-style models generate text
Features
Character-level tokenizer
Transformer decoder architecture
Self-attention implementation
Multi-head attention
Feed-forward neural networks
Positional embeddings
Layer normalization + residual connections
Text generation/sampling
PyTorch-based training pipeline
Tech Stack
Python
PyTorch
Jupyter Notebook / VS Code
NumPy
Matplotlib (optional for visualizations)
Model Architecture

The implementation follows the core transformer decoder structure used in GPT models:

Input Tokens
     ↓
Token Embeddings + Positional Embeddings
     ↓
Transformer Blocks
    ├── Multi-Head Self Attention
    ├── Feed Forward Network
    ├── Residual Connections
    └── Layer Normalization
     ↓
Linear Layer
     ↓
Softmax
     ↓
Predicted Next Token

The project starts with a simple bigram model before gradually building toward a mini GPT implementation.

Installation

Clone the repository:

git clone https://github.com/yourusername/gpt-from-scratch.git
cd gpt-from-scratch

Install dependencies:

pip install -r requirements.txt

Run training:

python train.py

Generate text:

python generate.py
What I’m Learning

This project is mainly focused on deeply understanding:

How transformers process sequences
Why attention works so well
Training dynamics of language models
Token prediction and autoregressive generation
Scaling from toy models to real-world LLM concepts

Acknowledgements

Huge credit to Andrej Karpathy for creating one of the best educational AI resources online and making advanced machine learning concepts approachable for everyone.

License

MIT License