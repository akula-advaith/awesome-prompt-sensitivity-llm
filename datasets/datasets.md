# Datasets

Relevant datasets for studying prompt sensitivity and LLM output stability.

## PromptSET

- **Source**: Built by Razavi et al. (2025) on top of TriviaQA and HotpotQA
- **Description**: A dataset purpose-built for the "Prompt Sensitivity Prediction" task — pairs original questions with multiple semantically-equivalent prompt variations, labeled by whether an LLM answers them consistently.
- **Application**: Training/evaluating models that predict *in advance* whether a given prompt is likely to be sensitive, without needing to query the LLM first.
- **Link**: [arXiv:2502.06065](https://arxiv.org/abs/2502.06065) (paper describing dataset construction)

## Big-Bench Hard (BBH)

- **Source**: Suzgun et al., BIG-bench collaborative benchmark suite
- **Description**: A curated subset of 23 challenging tasks from BIG-bench where prior LLMs underperformed human raters; widely reused as a testbed for measuring how much accuracy shifts under different prompt templates.
- **Application**: Used in prompt-sensitivity studies (e.g. POSIX, arXiv:2410.02185) to quantify template-induced accuracy variance across models.
- **Link**: [github.com/suzgunmirac/BIG-Bench-Hard](https://github.com/suzgunmirac/BIG-Bench-Hard)

## PromptRobust Adversarial Prompt Suite

- **Source**: Zhu et al. (2023), built on GLUE, MMLU, SQuAD V2, IWSLT 2017, and other standard NLP benchmarks
- **Description**: 4,788 adversarial prompt variants generated via character-, word-, sentence-, and semantic-level perturbations, applied across 8 tasks and 13 underlying datasets.
- **Application**: Stress-testing how robust a model's task performance is to superficial, meaning-preserving prompt perturbations.
- **Link**: [github.com/microsoft/promptbench](https://github.com/microsoft/promptbench)
