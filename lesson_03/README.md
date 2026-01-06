# Lesson 03: Sequence Modeling and Transformers

## Overview
We introduce autoregressive sequence modeling and the transformer architecture. The goal is to view LLMs as policies over tokens, with cross-entropy training and decoding as the core mechanics.

## Learning objectives
- Write the autoregressive factorization for sequences.
- Explain tokenization and the role of vocabulary design.
- Derive the cross-entropy objective for language modeling.
- Describe attention and transformer blocks at a high level.
- Compare decoding and sampling strategies used at inference time.

## Lesson structure
1. Autoregressive sequence modeling
   - Factorization of p(y) over tokens
   - Teacher forcing and likelihood
2. Tokenization and vocabulary
   - Subword models, BOS/EOS, context length
3. Cross-entropy objective
   - Negative log-likelihood and per-token loss
4. Attention mechanism
   - Queries, keys, values, self-attention
5. Transformer architecture
   - Multi-head attention, MLP blocks, residuals
   - Positional encoding
6. Decoding and sampling
   - Greedy, temperature, top-k, nucleus
7. LLM as a policy over tokens
   - Mapping to actions and trajectories

## Key terms
- autoregressive, cross-entropy, attention, transformer, tokenization, decoding

## Suggested prep
- Skim a transformer overview blog or paper summary.
