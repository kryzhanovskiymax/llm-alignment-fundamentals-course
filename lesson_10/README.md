# Lesson 10: Benchmarks and Evaluation for Aligned LLMs

## Overview
This lesson surveys evaluation practice for aligned LLMs: offline vs online evaluation, automatic vs human assessments, benchmark types, and checks for reward hacking or regressions.

## Learning objectives
- Distinguish offline evaluation from online or human-in-the-loop evaluation.
- Select benchmark suites based on task type and alignment goals.
- Validate reward models and detect over-optimization.
- Design regression tests and monitoring for deployed systems.

## Lesson structure
1. Evaluation taxonomy
   - Offline vs online, automatic vs human
2. Automatic metrics
   - Task accuracy, calibration, robustness
3. Human evaluation
   - Pairwise preference, rubric scoring
4. Benchmark families
   - Instruction-following, safety, reasoning
5. Reward model validation
   - Overfitting checks and holdout data
6. Reward hacking and distribution shift checks
   - Behavioral red-teaming
7. Regression testing
   - Golden prompts and continuous monitoring

## Key terms
- offline eval, online eval, human evaluation, benchmark, reward hacking, regression test

## Suggested prep
- Browse a recent alignment benchmark report or leaderboard.
