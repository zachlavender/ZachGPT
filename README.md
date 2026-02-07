# ZachGPT - LLM from Scratch

An educational project to build a Large Language Model from scratch using only NumPy.

## Overview

This project implements a transformer-based language model without relying on deep learning frameworks like PyTorch or TensorFlow. The goal is to understand the fundamental mechanics of modern LLMs by building every component from the ground up.

## Project Structure

```
ZachGPT/
├── notebooks/          # Jupyter notebook with all implementation
│   └── ZachGPT.ipynb  # Main notebook (all code lives here)
├── data/               # Training data (gitignored)
│   ├── raw/           # Original text datasets
│   └── processed/     # Tokenized/preprocessed data
├── checkpoints/        # Model checkpoints (gitignored)
├── logs/              # Training logs (gitignored)
└── requirements.txt    # Dependencies
```

## Setup

### Prerequisites

- Python 3.10+
- pip (comes with Python)

### Installation

1. Clone the repository
2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter:
   ```bash
   jupyter notebook notebooks/ZachGPT.ipynb
   ```

## Dependencies

- **NumPy**: Core numerical computing library
- **tiktoken**: GPT-2 tokenizer (OpenAI's BPE implementation)
- **Jupyter**: Interactive notebook environment
- **ipykernel**: Jupyter kernel for Python

## Goals

1. Build a transformer architecture from scratch
2. Implement self-attention mechanisms
3. Create tokenization and data processing pipelines
4. Train a small language model (10M-100M parameters)
5. Implement text generation capabilities

## Learning Objectives

- Deep understanding of transformer architecture
- Matrix operations and backpropagation
- Attention mechanisms (self-attention, multi-head attention)
- Layer normalization and residual connections
- Training dynamics and optimization
- Tokenization strategies

## Development Approach

This project uses a **notebook-first approach** for learning. All code, explanations, and experiments are contained in a single Jupyter notebook (`ZachGPT.ipynb`) that builds up the transformer from basics to a complete language model.

## Development Status

Current phase: Project setup complete, tokenization implemented

## Roadmap

- [x] Project initialization and setup
- [x] Explain tokenization concepts
- [ ] Implement basic math utilities in notebook (softmax, layer norm, etc.)
- [ ] Build embedding layers
- [ ] Implement attention mechanisms
- [ ] Create transformer architecture
- [ ] Build training loop
- [ ] Implement text generation
- [ ] Add evaluation metrics

## License

MIT License (or choose your preferred license)

## Acknowledgments

This project is for educational purposes, inspired by the foundational work on transformers and modern language models.
