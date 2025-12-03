# Lab 4 — Model Testing with Zeno & LLM-Driven Test Generation

##  Overview
This repository contains **my completed Lab 4** for the CMU SEAI course.  
It builds on the original starter repository but includes my own:
- Slice-based sentiment analysis
- LLM-driven test generation
- Accuracy evaluation before and after synthetic examples
- Polished Markdown documentation

##  Relation to Original Repo
This repo was forked from [cmu-seai/cmu-mlip-model-testing-lab](https://github.com/cmu-seai/cmu-mlip-model-testing-lab).  
All starter files remain, but I’ve added my completed lab work, updated notebooks, and documentation.

##  Contents
- `notebooks/` → Jupyter notebooks with slice definitions and evaluations
- `results/` → Accuracy tables and Markdown documentation
- `README.md` → Updated project overview
- `requirements.txt` → Environment dependencies (instead of committing `venv/`)

##  Key Insights
- Positive sentiment slices performed strongly (~95% accuracy).
- Negative and ambiguous slices revealed weaknesses in sarcasm and factual decline handling.
- Emoji slices showed robustness with explicit signals but need more testing with ambiguous emojis.
- Low confidence predictions reliably flagged unstable cases.

##  How to Run
Clone the repo and install dependencies:
```bash
git clone https://github.com/Leamota/Lab-4-Model-Testing-with-Zeno-LLM-Driven-Test-Generation.git
cd Lab-4-Model-Testing-with-Zeno-LLM-Driven-Test-Generation
pip install -r requirements.txt
