# Lesson 04: LLM Training Pipeline Overview

## Overview
This lesson walks through the end-to-end LLM alignment pipeline: pretraining, supervised fine-tuning, preference data and reward modeling, and RL fine-tuning with KL regularization. We also highlight common alignment failure modes that motivate RL.

## Learning objectives
- Describe each stage of the modern LLM training pipeline.
- Explain how preference data becomes a reward model.
- Understand why KL regularization appears in RL fine-tuning.
- Identify alignment failure modes that require RL-based methods.

## Lesson structure
1. Pretraining
   - Next-token prediction objective
   - Data scale and domain mix
2. Supervised fine-tuning (SFT)
   - Instruction tuning data
   - Behavior shaping vs generalization
3. Preference data and reward modeling
   - Pairwise preferences and ranking loss
   - Reward model calibration
4. RL fine-tuning
   - On-policy rollouts and PPO-style updates
   - KL penalty to a reference policy
5. Alignment failure modes
   - Reward hacking, mode collapse
   - Distribution shift and safety regressions

## Key terms
- pretraining, SFT, reward model, KL regularization, RLHF

## Suggested prep
- Read a short overview of RLHF or DPO-style pipelines.
