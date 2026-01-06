# Lesson 08: Effective Modern Alignment Methods (Aligned to Book)

## Overview
This lesson follows the book's chapter on effective policy optimization methods for LLM alignment. We formalize LLMs as MDPs, introduce group-based Monte-Carlo baselines, and cover GRPO, GSPO, SAPO, and related variants.

## Learning objectives
- Map token generation to an RL task with KL-regularized objectives.
- Use group-based Monte-Carlo baselines for critic-free advantages.
- Compare token-level vs sequence-level importance ratios.
- Explain GRPO, Dr. GRPO, DAPO, GSPO, and SAPO at the objective level.

## Lesson structure (aligned to book)
### 1. RL task setup for LLM alignment
- Tokens as actions, prefixes as states
- Reward model and KL-regularized objective
- On-policy iteration with a frozen behavior policy

### 2. Group-based Monte-Carlo baselines (critic-free advantages)
- Group sampling per prompt
- Group-normalized advantages
- Token and sequence importance ratios

### 3. Group Relative Policy Optimization (GRPO)
- Optimized surrogate objective
- Optimization algorithm (GRPO)

### 4. Modifications of GRPO
- Dr. GRPO (Group Relative Policy Optimization Done Right)
- DAPO: Decoupled Clip and Dynamic sAmpling Policy Optimization

### 5. Group Sequence Policy Optimization (GSPO)
- Token-level vs sequence-level importance ratios as change of measure
- GSPO objective (sequence-level clipping, reward alignment)
- Gradient comparison: GSPO vs GRPO
- Algorithm (GSPO)

### 6. Soft Adaptive Policy Optimization (SAPO)
- Setup: group sampling and critic-free advantages
- From GRPO hard clipping to a soft gate
- SAPO objective
- SAPO gradient and the gate interpretation
- Algorithm (SAPO)

## Key terms
- KL-regularized objective, group baseline, GRPO, Dr. GRPO, DAPO, GSPO, SAPO

## Suggested prep
- Review the book section "Effective Policy Optimization methods".
