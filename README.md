# LLM-Text-to-SQL-Thesis
Bachelor's thesis: systematic evaluation of Zero-Shot, Few-Shot and Chain-of-Thought prompting for Text-to-SQL on GeoQuery using Llama 3.3 70B Instruct

# Prompt Engineering for LLM-Based Text-to-SQL Translation

This repository contains the full implementation code and experimental results 
for the Bachelor's thesis *"Prompt Engineering for LLM-Based Text-to-SQL 
Translation: A Systematic Evaluation of Accuracy and Computational Efficiency 
on the GeoQuery Benchmark"*, submitted to LUISS Guido Carli, Department of 
Business Management, Chair of Database & Big Data (ING-INF/05), 
Academic Year 2025/2026.

**Author:** Francesca Peppoloni  
**Supervisor:** Prof. Blerina Sinaimeri

## Overview

This work systematically compares three prompt engineering strategies — 
Zero-Shot, Few-Shot and Chain-of-Thought — for the Text-to-SQL task, using 
Llama 3.3 70B Instruct on the GeoQuery benchmark (246 questions). 
Performance is evaluated on Execution Accuracy, Valid Efficiency Score 
and generation latency, alongside a per-category error analysis built on 
six failure modes.

## Repository Structure

- `notebooks/` — Jupyter notebook with the full evaluation pipeline
- `data/` — GeoQuery dataset (JSON) and SQLite database
- `results/` — CSV files with per-query results for each strategy
- `requirements.txt` — Python dependencies

## How to Reproduce

1. Clone the repository  
2. Install dependencies: `pip install -r requirements.txt`  
3. Create a `.env` file in the root directory and add your Groq API key:  
   `GROQ_API_KEY=your_key_here`  
4. Open the notebook and run the cells in order

## Headline Results

| Strategy          | Execution Accuracy | VES   | Avg. Generation Time |
|-------------------|-------------------:|------:|---------------------:|
| Zero-Shot         | 60.6%              | 56.5% | 3.11s                |
| Few-Shot          | 70.3%              | 72.1% | 3.91s                |
| Chain-of-Thought  | 77.6%              | 76.5% | 6.87s                |

## License

This project is released under the MIT License. The GeoQuery dataset 
retains its original license from Zelle & Mooney (1996).

## Contact

For questions about the implementation or the thesis, feel free to reach out.
