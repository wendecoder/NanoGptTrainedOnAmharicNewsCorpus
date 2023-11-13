# Amharic Text Generation with Transformer

This repository contains the implementation of a character-level text generation model for Amharic language using a Transformer architecture. The model is trained to replicate Amharic news-like text based on a provided dataset.

## Model Architecture

The Transformer model comprises the following components:

- **Positional Encoding:** Incorporates positional information into the input data.
- **Multi-Head Self-Attention:** Allows the model to weigh different parts of the input differently.
- **FeedForward Layer:** Applies a feedforward neural network to capture complex patterns.
- **Layer Normalization:** Normalizes the output of each sub-layer.

The model is a stack of decoder layers, each consisting of self-attention, feedforward, and normalization.

## Hyperparameters

- **Batch Size:** 64
- **Block Size:** 256
- **Max Iterations:** 5000
- **Evaluation Interval:** 500
- **Learning Rate:** 3e-4
- **Number of Embeddings (n_embd):** 384
- **Number of Attention Heads (n_head):** 6
- **Number of Transformer Layers (n_layer):** 6
- **Dropout:** 0.2

## Usage

1. Install the required dependencies:

   ```bash
   pip install torch torch-xla
   ```

2. Train the model:

   ```bash
   python train.py
   ```

3. Generate text using the trained model:

   ```bash
   python generate.py
   ```

## Dataset

The model is trained on an Amharic news dataset, and the training data is split into train and validation sets.

## Reference

The code structure and initial implementation were adapted from the [ng-video-lecture](https://github.com/karpathy/ng-video-lecture) repository by Andrej Karpathy.

## License

This project is licensed under the [MIT License](LICENSE).

---
