# Hugging Face LLM Course Journey

Hands-on notes and experiments while learning Transformers and LLMs, mainly from the [Hugging Face LLM Course](https://huggingface.co/learn/llm-course).

**Background:** actuary (ASAI) with 10+ years in life insurance and reinsurance analytics, moving into AI engineering. Each section contains runnable notebooks, my own notes, and small experiments beyond the course material.

## Progress

| Section | Topic | Notebook | What I did beyond the course | Status |
|---|---|---|---|---|
| 1.3 | Pipelines: what Transformers can do | [notebook](ch01_transformer_models_1_3_pipelines.ipynb) | Tested zero-shot classification with my own label sets; computed softmax manually to understand model scores; tuned `temperature` and `num_return_sequences` in text generation; compared a base generator's behaviour on direct questions | ✅ Done |
| 1.4 | How Transformers work | [notebook](ch01_transformer_models_1_4_how_do_transformers_work.ipynb) | Summarised Transformer history, encoder vs decoder vs encoder-decoder, transfer learning, attention, and architecture vs checkpoint; inspected BERT encoder output shape (`last_hidden_state`) | ✅ Done |
| 1.5 | How Transformers solve tasks | – | – | ⏳ Next |
| 2 | Using 🤗 Transformers | – | – | ⬜ |
| 3 | Fine-tuning a pretrained model | – | – | ⬜ |

## Key takeaways so far

- **Pretrained ≠ no training.** Ready-to-use models such as the default sentiment model are pretrained on raw text, then fine-tuned on labelled data by someone else.
- **Encoder vs decoder.** Encoders (BERT) are best for understanding and extraction; decoders (GPT, Llama, Qwen) are best for generation.
- **Architecture vs checkpoint.** The architecture is the code blueprint; the checkpoint is the trained weights downloaded from the Hub.
- **Model scores are softmax outputs.** Zero-shot and classification scores are raw logits converted into probabilities that sum to 1.

## Planned mini project

- **Treaty field extraction:** extract retention, limit, commission and period from *synthetic* reinsurance term sheets, comparing a regex baseline, an extractive QA model and an instruct LLM, with field-level accuracy evaluation.

## Tools

Python · Hugging Face Transformers · PyTorch · NumPy · Google Colab
