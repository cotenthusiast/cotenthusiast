<!--# Hi, I'm Karl -->>

CS student at Queen's University Belfast, doing machine learning research.

<!--I study the gap between how models are **measured** and how they actually **behave** — what happens when a model is moved outside the conditions it was trained or evaluated under.-->

[ORCID](https://orcid.org/0009-0000-0016-6121) · [LinkedIn](https://www.linkedin.com/in/karl-hanna-88919a396/) · [arXiv](https://arxiv.org/a/hanna_k_1) <!-- TODO: check arXiv author-page URL; add email if you want recruiters to reach you -->

**Currently:** looking for a 12-month ML research / research engineering placement starting June 2027 / September 2027.

---

## Research

### [Amadeus Counterpoint](https://github.com/cotenthusiast/amadeus-counterpoint): *What happens when models of people meet?*

If you model two people separately, each learned only from their interactions with *other* people, can you put the two models together and reproduce how they interact with **each other**?

Chess is the controlled testbed: eight elite players, with every direct game between a pair held out during training.

<!-- TODO: one sentence with the headline result, e.g. "Composed player models recover X of the held-out pair's behaviour, measured by Y." -->

- Trained a 77.8M-parameter transformer from scratch with player-specific behavioural representations
- Leave-one-opponent-out training and held-out dyadic evaluation, run on SLURM/HPC

**Python · PyTorch · SLURM/HPC** · Independent research · Under review
[Code](https://github.com/cotenthusiast/amadeus-counterpoint) · Paper <!-- TODO: arXiv link once live -->

<!-- TODO: one figure (e.g. the held-out dyad setup or the main results plot) -->

---

### [ChoiceBench](https://github.com/cotenthusiast/choicebench): *A model can be accurate without being consistent*

LLM multiple-choice scores mix up knowledge with sensitivity to the order the options appear in. Hiding option labels while the model commits to an answer, or scoring each option in isolation (unbiased by construction), does **not** reliably improve accuracy, while cyclic permutation often does. Removing positional influence and gaining accuracy turn out to be different things.

- Built the evaluation framework: multiple answering strategies, benchmarks, hosted and local models, reproducible HPC runs
- Reproduced Zheng et al. (ICLR 2024) PriDe results at full MMLU scale (13,564 questions)
- Six models across MMLU and ARC-Challenge, with exact and bootstrap confidence intervals and per-question flip rates

**Python · PyTorch · Hugging Face · vLLM · SLURM/HPC**
[Paper](https://arxiv.org/abs/2608.11947) · [Code](https://github.com/cotenthusiast/choicebench)

<!-- TODO: one figure (e.g. accuracy vs order sensitivity per strategy) -->

---

## Papers

- **K. Hanna**, C. Feng. *Accuracy and Order Sensitivity Diverge Under Label-Free Strategies.* arXiv:2608.11947, 2026. [[paper]](https://arxiv.org/abs/2608.11947) [[code]](https://github.com/cotenthusiast/choicebench)
- **K. Hanna.** *Amadeus: When Models of People Meet.* Under review, 2026. [[paper]](https://arxiv.org/abs/2608.11947) [[code]](https://github.com/cotenthusiast/amadeus-counterpoint) 

---

## Built from scratch

| Project | What it is |
|---|---|
| [mini-gpt](https://github.com/cotenthusiast/mini-gpt) + [BPE-tokenizer](https://github.com/cotenthusiast/BPE-tokenizer) | Byte-pair tokeniser and decoder-only transformer, to understand the language-modelling stack end to end |
| [neural-network-from-scratch](https://github.com/cotenthusiast/neural-network-from-scratch) | NumPy MLP on Fashion-MNIST: forward/backward pass, optimisation, checkpointing, controlled experiments |
| [susume](https://github.com/cotenthusiast/susume) | Anime recommender exploring collaborative filtering and matrix factorisation |

---

**ML & research:** PyTorch · NumPy · Hugging Face · vLLM
**Languages:** Python · Java · C++  · Bash
**Infrastructure:** Linux · SLURM/HPC · Git · LaTeX
