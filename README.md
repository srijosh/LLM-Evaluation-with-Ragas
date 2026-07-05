# LLM Evaluation with Ragas

This repository contains an interactive Jupyter Notebook demo for evaluating a RAG (Retrieval-Augmented Generation) system using RAGAS. The notebook is designed to help you measure how well an LLM-powered retrieval pipeline performs across common failure modes such as hallucination, irrelevance, weak context retrieval, and incorrect answers.

The project is notebook-first and intended for hands-on experimentation with:

- RAGAS-based evaluation of LLM responses
- retrieval and generation quality measurement
- local embedding support with sentence-transformers
- Groq or OpenAI-based judge models for scoring
- mock datasets that isolate specific RAG issues

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Tools and Technologies](#tools-and-technologies)

## Introduction

This project focuses on evaluating LLM systems rather than just building them. It demonstrates how to assess a RAG workflow using RAGAS metrics such as:

- Faithfulness
- Answer Relevancy
- Context Precision
- Context Recall
- Answer Correctness
- Tool Correctness

The notebook walks through a practical evaluation setup using mock examples and a judge LLM, making it easier to understand where a RAG pipeline may fail.

## Features

- Evaluate retrieval quality and response quality with RAGAS
- Measure six important RAG failure modes in one workflow
- Use local embeddings with sentence-transformers
- Connect a Groq or OpenAI-backed judge model for scoring
- Separate evaluation logic from generation logic for easier experimentation

## Installation

1. Clone the repository:

```bash
git clone https://github.com/srijosh/LLM-Evaluation-with-Ragas.git
```

2. Navigate to the project directory:

```bash
cd LLM-Evaluation-with-Ragas
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Set up environment variables by creating a `.env` file from `.env.sample`.

## Usage

Open the notebook and run the cells in order:

```bash
jupyter notebook evals.ipynb
```

## Tools and Technologies

- **RAGAS**: automated framework for retrieval-augmented generation evaluation
- **LangChain**: LLM workflow orchestration and component integration
- **Groq API**: high-speed inference engine for running open-source LLMs
- **python-dotenv**: environment variable management and API key loading
- **sentence-transformers**: local embedding generation for semantic search and evaluation
