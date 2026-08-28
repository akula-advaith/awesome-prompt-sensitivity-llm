# References — Curated & Verified

All references below were independently verified against DOI/Crossref, arXiv, ACL Anthology, or the publisher record, per the citation-integrity audit process. A note on exclusions/corrections is at the bottom.

## A. Foundational Prompting & Reasoning Methods

- **Calibrate Before Use: Improving Few-Shot Performance of Language Models**
  Zhao, Z., Wallace, E., Feng, S., Klein, D. & Singh, S., 2021, ICML
  [arXiv:2102.09690](https://arxiv.org/abs/2102.09690)
  Foundational work showing that few-shot LLM performance is highly sensitive to prompt/example choice — a root motivation for studying prompt sensitivity.

- **Fantastically Ordered Prompts and Where to Find Them: Overcoming Few-Shot Prompt Order Sensitivity**
  Lu, Y., Bartolo, M., Moore, A., Riedel, S. & Stenetorp, P., 2022, ACL
  [DOI: 10.18653/v1/2022.acl-long.556](https://doi.org/10.18653/v1/2022.acl-long.556) · [arXiv:2104.08786](https://arxiv.org/abs/2104.08786)
  Shows that the mere ordering of few-shot examples in a prompt can swing accuracy dramatically — an early, direct demonstration of prompt sensitivity.

- **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models**
  Wei, J., Wang, X., Schuurmans, D., Bosma, M., Ichter, B., Xia, F., Chi, E., Le, Q. V. & Zhou, D., 2022, NeurIPS
  [arXiv:2201.11903](https://arxiv.org/abs/2201.11903)
  Establishes chain-of-thought prompting as a technique whose presence/absence materially changes model conclusions — relevant baseline for reasoning-stability discussions.

- **Large Language Models are Zero-Shot Reasoners**
  Kojima, T., Gu, S. S., Reid, M., Matsuo, Y. & Iwasawa, Y., 2022, NeurIPS
  [arXiv:2205.11916](https://arxiv.org/abs/2205.11916)
  Demonstrates that a single added phrase ("Let's think step by step") changes reasoning outcomes — a minimal, clean example of prompt-wording sensitivity.

- **Self-Consistency Improves Chain of Thought Reasoning in Language Models**
  Wang, X., Wei, J., Schuurmans, D., Le, Q. V., Chi, E. H., Narang, S., Chowdhery, A. & Zhou, D., 2023, ICLR
  [arXiv:2203.11171](https://arxiv.org/abs/2203.11171)
  Proposes sampling multiple reasoning paths to stabilize conclusions — directly relevant to mitigating prompt-induced instability.

## B. Prompt Sensitivity & Robustness — Core Topic

- **ProSA: Assessing and Understanding the Prompt Sensitivity of LLMs**
  Zhuo, J., Zhang, S., Fang, X., Duan, H., Lin, D. & Chen, K., 2024, Findings of ACL: EMNLP 2024
  [DOI: 10.18653/v1/2024.findings-emnlp.108](https://doi.org/10.18653/v1/2024.findings-emnlp.108)
  Introduces PromptSensiScore, a dedicated metric for quantifying prompt sensitivity — central methodological reference for this topic.

- **What Did I Do Wrong? Quantifying LLMs' Sensitivity and Consistency to Prompt Engineering**
  Errica, F., Sanvito, D., Siracusano, G. & Bifulco, R., 2025, NAACL-HLT
  [DOI: 10.18653/v1/2025.naacl-long.73](https://doi.org/10.18653/v1/2025.naacl-long.73)
  Proposes sensitivity and consistency measures for classification tasks under prompt rephrasing.

- **Flaw or Artifact? Rethinking Prompt Sensitivity in Evaluating LLMs**
  Hua, A., Tang, K., Gu, C., Gu, J., Wong, E. & Qin, Y., 2025, EMNLP
  [DOI: 10.18653/v1/2025.emnlp-main.1006](https://doi.org/10.18653/v1/2025.emnlp-main.1006)
  Questions whether observed "sensitivity" reflects genuine model fragility or evaluation-pipeline artifacts — directly relevant to interpreting stability results.

- **Understanding the Prompt Sensitivity**
  Liu, Y. & Chu, C., 2026, arXiv
  [arXiv:2604.18389](https://arxiv.org/abs/2604.18389)
  Uses a Taylor-expansion, function-based framing of LLMs to give a theoretical account of why prompt sensitivity occurs.

- **Evaluating and Explaining Prompt Sensitivity of LLMs Using Interactions**
  Qin, R., Wang, Q., Wang, T., Wei, Z. & Shen, W., 2026, ICML
  [arXiv:2608.18539](https://arxiv.org/abs/2608.18539)
  Interaction-based framework for explaining *why* certain prompts trigger instability, not just measuring that they do. *(Note: the source paper cited OpenReview ID `GsdFM8qnav`; the correct ID is `6fHZR6uxNa` — corrected here after verification.)*

- **PromptBench / PromptRobust: Towards Evaluating the Robustness of Large Language Models on Adversarial Prompts**
  Zhu, K., Wang, J., Zhou, J., Wang, Z., Chen, H., Wang, Y., Yang, L., Ye, W., Gong, N. Z., Zhang, Y. & Xie, X., 2023
  [arXiv:2306.04528](https://arxiv.org/abs/2306.04528)
  Introduces a large-scale adversarial-prompt benchmark (4,788 prompts, 8 tasks) — the standard reference point for prompt robustness evaluation.

- **Quantifying Language Models' Sensitivity to Spurious Features in Prompt Design (or: How I Learned to Start Worrying About Prompt Formatting)**
  Sclar, M., Choi, Y., Tsvetkov, Y. & Suhr, A., 2024, ICLR
  [arXiv:2310.11324](https://arxiv.org/abs/2310.11324)
  Shows formatting-only changes (delimiters, whitespace) can shift accuracy by up to 76 points — a striking, widely-cited demonstration of sensitivity.

- **How are Prompts Different in Terms of Sensitivity?**
  Lu, S., Schuff, H. & Gurevych, I., 2024, NAACL-HLT
  [DOI: 10.18653/v1/2024.naacl-long.325](https://doi.org/10.18653/v1/2024.naacl-long.325)
  Uses gradient-based saliency to show sensitivity is an unsupervised proxy that correlates negatively with model accuracy.

- **Benchmarking Prompt Sensitivity in Large Language Models**
  Razavi, A., Soltangheis, M., Arabzadeh, N., Salamat, S., Zihayat, M. & Bagheri, E., 2025, ECIR
  [DOI: 10.1007/978-3-031-88714-7_29](https://doi.org/10.1007/978-3-031-88714-7_29)
  Introduces the Prompt Sensitivity Prediction task and the PromptSET dataset (built on TriviaQA/HotpotQA).

## C. Factuality, Reliability & Prompting Surveys

- **TruthfulQA: Measuring How Models Mimic Human Falsehoods**
  Lin, S., Hilton, J. & Evans, O., 2022, ACL
  [DOI: 10.18653/v1/2022.acl-long.229](https://doi.org/10.18653/v1/2022.acl-long.229)
  Standard benchmark for measuring factual reliability of LLM outputs — relevant baseline for assessing "stability of conclusions."

- **Factuality Enhanced Language Models for Open-Ended Text Generation**
  Lee, N., Ping, W., Xu, P., Patwary, M., Fung, P., Shoeybi, M. & Catanzaro, B., 2022, NeurIPS
  [arXiv:2206.04624](https://arxiv.org/abs/2206.04624)
  Proposes decoding-side interventions to improve factual consistency in generated text.

- **The Prompt Report: A Systematic Survey of Prompting Techniques**
  Schulhoff, S., Ilie, M., Balepur, N. et al., 2024, arXiv
  [arXiv:2406.06608](https://arxiv.org/abs/2406.06608)
  Large-scale systematic survey cataloguing prompting techniques — useful reference map for the field.

## D. Reproducibility & Applied Research Methodology

- **Reproducibility in NLP: What Have We Learned from the Checklist?**
  Magnusson, I., Smith, N. A. & Dodge, J., 2023, Findings of ACL
  [arXiv:2306.09562](https://arxiv.org/abs/2306.09562)
  Examines reproducibility failures in NLP research — connects prompt instability to the broader reproducibility crisis in AI-assisted research.

- **Designing GPT3 Prompts to Screen Articles for Systematic Reviews of RCTs**
  Strachan, J. A., 2024, Health Policy and Technology
  [DOI: 10.1016/j.hlpt.2024.100943](https://doi.org/10.1016/j.hlpt.2024.100943)
  Applied case study of prompt design affecting real research-screening decisions — grounds the topic in a concrete research-conclusions use case.

- **Think Through Uncertainty: Improving Long-Form Generation Factuality via Reasoning Calibration**
  Liu, X. & Wang, L., 2026, arXiv
  [arXiv:2604.12046](https://arxiv.org/abs/2604.12046)
  Proposes calibrating reasoning under uncertainty to improve factuality of long-form generations.

- **Evaluating Prompting Strategies and Large Language Models in Systematic Literature Review Screening: Relevance and Task-Stage Classification**
  Han, B., Mathrani, A. & Susnjak, T., 2025, arXiv
  [arXiv:2510.16091](https://arxiv.org/abs/2510.16091)
  Evaluates how different prompting strategies affect LLM reliability in a real research-screening pipeline.

---

## Verification Note

This list draws on the citation-integrity audit conducted for this project (see `citation-audit/`). Of 18 references originally generated by an AI assistant for the underlying paper:
- **16 were fully verified** (correct title, authors, year, venue, and identifier)
- **1 had a corrected identifier** — Qin et al. (2026): real paper, but the originally cited OpenReview ID was wrong (corrected above)
- **1 was found to be fabricated and is excluded from this repository**: "Leng, Y. (2026). When Prompts Matter... SSRN working paper" — no trace of this publication could be found across SSRN, Google Scholar, or general web search.

Four additional papers (PromptBench, Sclar et al., Lu/Schuff/Gurevych, and Razavi et al.) were independently sourced and verified to round out this collection past the 20-paper minimum.
