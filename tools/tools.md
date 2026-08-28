# Tools & Libraries

Software tools useful for testing, evaluating, and mitigating prompt sensitivity in LLMs.

- **[promptfoo](https://github.com/promptfoo/promptfoo)**
  Open-source CLI/library for systematically testing and comparing prompt variations across LLM providers; produces matrix views to catch prompt-induced output regressions before they reach production.

- **[lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)** (EleutherAI)
  The standard framework for running LLMs against academic benchmarks in a reproducible, standardized way — useful for controlling for prompt/template variance when comparing models.

- **[DSPy](https://github.com/stanfordnlp/dspy)**
  A programming framework that treats prompts as compiled, optimizable artifacts rather than hand-written strings, aiming to reduce fragile manual prompt engineering.

- **[Guidance](https://github.com/guidance-ai/guidance)**
  A templating/control library for constraining and structuring LLM generation, reducing variance introduced by unconstrained free-form prompting.

- **[LangChain](https://github.com/langchain-ai/langchain)**
  Widely-used framework offering prompt templates, output parsers, and evaluation utilities; commonly used as infrastructure in prompt-sensitivity experiments.
