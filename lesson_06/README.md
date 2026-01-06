# Lesson 06: Policy Gradient Methods (Aligned to Book)

## Overview
This lesson follows the book's policy optimization chapter. We derive the policy gradient theorem, implement vanilla policy gradient, and cover common variance-reduction techniques including baselines and actor-critic methods.

## Learning objectives
- Derive the policy gradient theorem using the log-derivative trick.
- Implement the vanilla policy gradient algorithm with reward-to-go.
- Use baselines and advantages to reduce variance.
- Explain A2C and A3C at the estimator level.

## Lesson structure (aligned to book)
### 1. Objective
- Define J(theta) for a parameterized policy

### 2. Policy gradient theorem
- Trajectory log-derivative form
- Reward-to-go form
- Discounted occupancy form with Q^pi

### 3. Basic policy optimization algorithm (Vanilla policy gradient)
- Sampling step
- Return computation
- Gradient estimator
- Parameter update

### 4. Improvements for gradient stability
- Baseline (control variate)
- A2C (Advantage Actor-Critic)
  - Critic update via TD error
  - Actor update with advantage estimates
- A3C (Asynchronous Advantage Actor-Critic)
  - Parallel sampling and asynchronous updates

## Key terms
- policy gradient, REINFORCE, reward-to-go, baseline, advantage, A2C, A3C

## Suggested prep
- Review the book section "Policy Optimization" up to "Improvements for gradient stability".
