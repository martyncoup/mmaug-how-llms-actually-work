# How Large Language Models Actually Work (Without the Hype)

An MMAUG Bootcamp session about what large language models do, how they learn, and how to use them with clear expectations.

**15 October 2026 at 18:00 CEST**  
**Speaker:** Martyn Coupland  
**Event:** [MMAUG Bootcamp](https://mmaug.com/bootcamp)

## Session description

Large language models have become everyday tools, but few people understand what's happening under the hood. This session explains how LLMs actually work, using plain language and accessible analogies instead of jargon.

We'll explore the core concept that these are sophisticated prediction engines learning patterns from vast amounts of text, and walk through what happens during training, how they process language, and why they behave the way they do. You'll leave understanding both their genuine capabilities and real limitations, with a practical mental model for using and evaluating these systems effectively.

## Learning objectives

By the end of the session, participants should be able to:

- Describe an LLM as a model that predicts likely next tokens from context, rather than as a database or a human-like mind.
- Explain, at a high level, how text is converted into tokens and numbers, how a neural network learns patterns during training, and how it generates an answer during inference.
- Recognise the roles of tokens, embeddings, context windows, attention, parameters, training data, and fine-tuning without needing to implement them.
- Distinguish pre-training, instruction tuning, and user prompting as different stages in shaping model behaviour.
- Explain why the same prompt can produce different answers and why fluent language is not evidence that an answer is true.
- Identify common failure modes, including hallucination, bias, missing or outdated knowledge, prompt sensitivity, and context limitations.
- Evaluate an LLM response using evidence, reproducible prompts, alternative checks, and an appropriate level of human review.
- Choose sensible use cases for LLMs and recognise when a deterministic program, search, or a subject-matter expert is a better fit.

## The mental model

An LLM is a very large mathematical model that has learned statistical patterns in language. Given the text so far, it estimates what tokens could come next and repeatedly selects one to continue the response.

That simple description explains both sides of the technology:

- **Why it is useful:** language patterns encode a surprising amount of structure, style, and general knowledge, so the model can summarise, transform, explain, and generate text or code.
- **Why it needs supervision:** the model is optimising for plausible continuation, not independently checking whether every statement is accurate, current, safe, or appropriate.

## Suggested flow

1. What an LLM is, and what it is not
2. From text to tokens and numbers
3. Training: learning patterns by predicting missing or next tokens
4. Inference: generating a response one token at a time
5. Attention, context, and why prompts matter
6. Capabilities, limitations, and common failure modes
7. A practical checklist for using and evaluating LLM output

## Useful links

### Start here

- [MMAUG Bootcamp](https://mmaug.com/bootcamp) - the programme page and schedule.
- [MMAUG Bootcamp curriculum](https://github.com/MMAUG-ORG/mmaug-bootcamp-2026) - the wider beginner-friendly learning path.
- [AI: A Guide for Thinking Humans](https://www.understandingai.org/) - a plain-language introduction to what modern AI systems can and cannot do.

### Visual explanations

- [But what is a GPT?](https://www.youtube.com/watch?v=wjZofJX0v4M) - 3Blue1Brown's visual explanation of language models and next-token prediction.
- [Attention in transformers, visually explained](https://www.youtube.com/watch?v=eMlx5fFNoYc) - an accessible introduction to the attention mechanism.
- [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) - a visual walkthrough of the Transformer architecture.

### Try the concepts

- [OpenAI Tokenizer](https://platform.openai.com/tokenizer) - see how text is split into tokens.
- [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) - a free path from transformer concepts to practical model use.
- [Google's Introduction to Large Language Models](https://developers.google.com/machine-learning/resources/intro-llms) - a concise introductory course covering the basics and responsible use.

### Reliability and responsible use

- [OpenAI: Why language models hallucinate](https://openai.com/index/why-language-models-hallucinate/) - why plausible answers can still be unsupported or wrong.
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) - a structured way to think about managing AI risks.
- [Microsoft Responsible AI](https://www.microsoft.com/en-us/ai/responsible-ai) - principles and practices for developing and using AI responsibly.

## Questions to ask when using an LLM

- What evidence supports this answer?
- Could the information be outdated, incomplete, or biased?
- What would happen if the answer were wrong?
- Can I verify it with a reliable source or a second method?
- Should a person review this before it is used or acted upon?

## Further reading

- Vaswani et al., [Attention Is All You Need](https://arxiv.org/abs/1706.03762) - the original Transformer paper.
- Brown et al., [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) - the GPT-3 paper and an influential discussion of in-context learning.
- [Stanford AI Index](https://aiindex.stanford.edu/report/) - annual data and analysis about AI capabilities, adoption, and impact.