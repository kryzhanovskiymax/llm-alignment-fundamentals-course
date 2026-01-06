# Lesson 02: Deep Learning Essentials

## Overview
This lesson covers core deep learning mechanics that later affect RL stability: neural networks, backpropagation, initialization, normalization, and regularization. We also discuss high-level scaling laws and why gradient variance matters for policy optimization.

## Learning objectives
- Explain feedforward networks, activation functions, and representation learning.
- Trace backpropagation with the chain rule.
- Understand vanishing/exploding gradients and why initialization matters.
- Compare normalization and regularization techniques.
- Connect scaling laws and gradient variance to RL training.

## Lesson structure
1. Neural networks as function approximators
   - Layers, activations, forward pass
   - Capacity and inductive bias
2. Backpropagation basics
   - Computational graphs and chain rule
   - Gradients as signals for learning
3. Optimization dynamics
   - Vanishing and exploding gradients
   - Learning rate sensitivity
4. Initialization and normalization
   - Xavier/He initialization
   - Batch norm vs layer norm
5. Regularization
   - Weight decay, dropout, early stopping
6. Scaling laws intuition
   - Data, model size, compute tradeoffs
7. Why gradient variance matters for RL
   - High variance updates and stability issues

## Key terms
- MLP, activation, backprop, initialization, normalization, regularization, scaling laws

## Suggested prep
- Review of derivatives and matrix notation.
