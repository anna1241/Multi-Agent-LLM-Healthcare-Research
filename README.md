# Multi-Agent LLM Healthcare Research Assistant

This project implements a Multi-Agent Autonomous Research Assistant using LangGraph and Large Language Models (LLMs) to automate healthcare-related research tasks. The system conducts keyword expansion, paper retrieval, ranking, summarization, comparative analysis, and generates a comprehensive research report — showcasing the power of LLMs in healthcare research automation.

## Features

- **Keyword Expansion:** Expands user queries into related keywords using a BART-based model.
- **Paper Retrieval:** Fetches relevant papers from arXiv using expanded keywords.
- **Paper Ranking:** Prioritizes papers by publication year and abstract length.
- **Summarization:** Generates summaries, key findings, and methodology insights using a fine-tuned DistilBART model.
- **Comparative Analysis:** Identifies common themes, contradictions, and gaps using BART-large.
- **Report Generation:** Creates a structured `.docx` report via `python-docx`.

## 🧠 Models Used

- `sshleifer/distilbart-cnn-12-6` (LoRA fine-tuned) → summarization
- `facebook/bart-base` → keyword expansion
- `facebook/bart-large-cnn` → comparative analysis
- `arXiv API` → paper retrieval
