# Hugging Face LLM Course Journey

My hands-on notes and experiments while learning Transformers and LLMs, mainly from the [Hugging Face LLM Course](https://huggingface.co/learn/llm-course).

Background: actuary (ASAI) with 10+ years in life insurance and reinsurance analytics, moving into data and AI engineering. Each chapter includes my own notes and at least one experiment applied to insurance or reinsurance use cases.

## Progress

| Chapter | Topic | Notebook | Own experiment | Status |
|---|---|---|---|---|
| 1.3 | Pipelines: what Transformers can do | [notebook](ch01-transformer-models/1.3-pipelines.ipynb) | Extract treaty fields with QA pipeline | ✅ Done |
| 1.4 | How Transformers work | – | – | ⏳ Next |
| 2 | Using 🤗 Transformers | – | – | ⬜ |
| 3 | Fine-tuning a pretrained model | – | – | ⬜ |

## Repo structure

```
hf-llm-course-journey/
├── README.md
├── ch01-transformer-models/
│   ├── 1.3-pipelines.ipynb
│   └── 1.3-notes.md
├── ch02-using-transformers/
├── ch03-fine-tuning/
└── mini-projects/
    └── treaty-field-extraction/
```

## Mini projects

- **Treaty field extraction** (planned): extract retention, limit, commission and period from synthetic reinsurance term sheets, comparing regex, extractive QA and an instruct LLM.

## Tools

Python · Hugging Face Transformers · PyTorch · Google Colab
