# Lesson 07: Bounded Policy Optimization (Aligned to Book)

## Overview
This lesson follows the book's bounded policy optimization chapter. We study why naive policy updates fail, derive conservative objectives, and connect them to TRPO and PPO.

## Learning objectives
- Explain distribution shift and importance sampling pathologies in policy updates.
- Use the Performance Difference Lemma to compare policies.
- Derive local surrogate objectives and distribution shift penalties.
- Understand CPI, TRPO, and PPO as bounded update methods.

## Lesson structure (aligned to book)
### 1. Motivation for bounded updates
- Why large policy steps destabilize on-policy estimates

### 2. Why naive policy optimization can fail: two toy pathologies
- Example 1: local surrogate predicts improvement but true performance collapses
- Example 2: trajectory importance sampling variance grows exponentially

### 3. Performance Difference Lemma
- Exact performance gap identity

### 4. Local surrogate objective and distribution shift penalty
- On-policy surrogate vs true objective

### 5. Conservative Policy Update
- Trusting the surrogate within a bounded step

### 6. Conservative Policy Iteration
- Iterative conservative updates

### 7. Trust Region Policy Optimization (TRPO)
- Parameterized policies and the trust-region problem
- Sample-based objective and constraint
- Efficient approximate solution (natural-gradient style step)
- Algorithm (TRPO)

### 8. Proximal Policy Optimization (PPO)
- Bounded-policy-optimization objective in parameter space
- Clipped PPO objective (policy loss)
- Full PPO objective (actor-critic form)
- Algorithm (PPO)

## Key terms
- distribution shift, Performance Difference Lemma, CPI, TRPO, PPO, KL constraint

## Suggested prep
- Review the book section "Bounded Policy Optimization".
