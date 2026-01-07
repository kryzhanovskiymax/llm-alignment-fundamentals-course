# Mathematical Fundamentals of Reinforcement Learning for LLM Alignment

This repository contains a 12-lesson course that builds the mathematical foundations needed to understand and implement modern reinforcement-learning-based alignment methods for large language models (LLMs).

**High-level flow**
- **Lessons 1–4:** Intro to ML, DL, and LLMs (enough to understand where RL/alignment fits and what the “policy” is).
- **Lessons 5–8:** Core mathematical RL + policy optimization, culminating in modern alignment methods (these lessons track the included book draft).
- **Lessons 9–10:** Practical aspects: tooling/systems and evaluation/benchmarks.
- **Lessons 11–12:** Reading group sessions (topics chosen dynamically).

---

## Course roadmap

| Lesson number | Lesson Name | Lesson Description | Link to slides | Link to conspect |
|---:|---|---|---|---|
| 1 | [ML foundations for alignment](lesson_01/README.md) | Supervised learning setup, loss functions, train/val/test, generalization intuition, basic optimization (SGD), probabilistic notation used throughout the course. | [Slides](lesson_01/slides/) | [Conspect](lesson_01/conspect.md) |
| 2 | [Deep Learning essentials](lesson_02/README.md) | Neural networks, backprop, initialization, regularization, normalization, scaling laws intuition (high-level), why gradients/variance matter for RL later. | [Slides](lesson_02/slides/) | [Conspect](lesson_02/conspect.md) |
| 3 | [Sequence modeling + Transformers](lesson_03/README.md) | Autoregressive modeling, cross-entropy objective, attention/transformers, tokenization, decoding/sampling basics needed to view LLMs as policies. | [Slides](lesson_03/slides/) | [Conspect](lesson_03/conspect.md) |
| 4 | [LLM training pipeline overview](lesson_04/README.md) | Pretraining -> SFT -> preference data/reward modeling -> RL Alignment techniques; Reward Design for preference data; alignment failure modes motivating RL. | [Slides](lesson_04/slides/) | [Conspect](lesson_04/conspect.md) |
| 5 | [RL fundamentals](lesson_05/README.md) | Probability/expectation review, Monte Carlo estimation, importance sampling basics, MDPs, trajectories, returns, discounted occupancy, value functions, TD idea. | [Slides](lesson_05/slides/) | [Conspect](lesson_05/conspect.md) |
| 6 | [Policy Gradient methods](lesson_06/README.md) | Log-derivative trick, REINFORCE, reward-to-go, baselines/control variates, actor-critic (A2C/A3C), advantage estimation as variance reduction. | [Slides](lesson_06/slides/) | [Conspect](lesson_06/conspect.md) |
| 7 | [Bounded optimization methods](lesson_07/README.md) | Performance Difference Lemma, local surrogate objective, distribution shift penalty, conservative policy updates (CPI), trust regions and KL constraints, TRPO mechanics. | [Slides](lesson_07/slides/) | [Conspect](lesson_07/conspect.md) |
| 8 | [Effective modern alignment methods](lesson_08/README.md) | LLM-as-MDP formalization (tokens/actions), KL-regularized objectives vs reference model, PPO-style clipping, critic-free/group baselines, GRPO + variants (DrGRPO/DAPO), sequence-level alternatives (GSPO), soft gating (SAPO). | [Slides](lesson_08/slides/) | [Conspect](lesson_08/conspect.md) |
| 9 | [Practical alignment tooling & systems](lesson_09/README.md) | Practical pipeline: data -> sampling -> scoring/reward -> optimization; common tooling patterns (training loops, rollout engines like vLLM, distributed execution, LoRA/PEFT), logging/monitoring, reproducibility. | [Slides](lesson_09/slides/) | [Conspect](lesson_09/conspect.md) |
| 10 | [Benchmarks & evaluation for aligned LLMs](lesson_10/README.md) | Offline eval vs online, automatic vs human eval, benchmark types (instruction-following, safety, reasoning), preference-model validation, reward hacking checks, regression testing. | [Slides](lesson_10/slides/) | [Conspect](lesson_10/conspect.md) |
| 11 | [Reading Group I](lesson_11/README.md) | (Reading group session; papers/topics TBD.) | [Slides](lesson_11/slides/) | [Conspect](lesson_11/conspect.md) |
| 12 | [Reading Group II](lesson_12/README.md) | (Reading group session; papers/topics TBD.) | [Slides](lesson_12/slides/) | [Conspect](lesson_12/conspect.md) |

---

## Book sources (Lessons 5–8)

The draft book *“RL Foundations for LLM Alignment”* is stored in:

- `materials/book/src.tex` — LaTeX source
- `materials/book/LLM_alignment_book.pdf` — compiled PDF (optional but recommended)

Lessons **5–8** are designed to match the book chapters:
- **L5:** core probability + RL fundamentals
- **L6:** policy gradients and actor–critic
- **L7:** bounded optimization (CPI/TRPO/PPO theory)
- **L8:** modern LLM alignment methods (PPO/GRPO-style and beyond)

---

## Suggested “minimum deliverables” per lesson folder

Each `lesson_XX/` should ideally contain:
- `README.md` (objectives, outline, reading, homework)
- `slides/`
- `conspect.md` (the compact mathematical notes)

Optional:
- `exercises/` (problem sets)
- `notebooks/` (implementation demos)
- `reading/` (paper list + annotations)
