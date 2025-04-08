# Hybrid LLM-Based Thematic Analysis Pipeline

This repository contains a modular pipeline for conducting inductive thematic analysis using large language models (LLMs). The method supports hybrid human-AI workflows and is model-agnostic, currently outlined for four different pre-trained LLMs: GPT-4, Mistral, LLaMA, and DeepSeek.

## Context

This project was developed as part of my Master’s thesis in the "Applied Data Information & Science program at Lucerne University of Applied Sciences and Arts (HSLU)". The aim of the thesis is to explore the capabilities and limitations of LLMs in supporting qualitative research tasks such as thematic analysis.

The pipeline draws conceptual inspiration from the following foundational studies:

- **Raza et al. (2025)** – *LLM-TA: An LLM-Enhanced Thematic Analysis Pipeline for Transcripts from Parents of Children with Congenital Heart Disease*
- **Katz et al. (2024a)** – *Thematic Analysis with Open-Source Generative AI and Machine Learning: A New Method for Inductive Qualitative Codebook Development*
- **De Paoli (2024)** – *Performing an Inductive Thematic Analysis of Semi-Structured Interviews With a Large Language Model: An Exploration and Provocation on the Limits of the Approach*

## Overview

The notebook illustrates a simplified and modular version of a thematic analysis workflow. It highlights key steps such as:

- Text/transcript chunking and preparation
- Prompting strategies for different stages (code generation, theme abstraction)
- NLP components like embedding and clustering approaches

> **Note:** The notebook is not a complete, ready-to-run pipeline. It requires:
> - Manual loading of your own textual data and its structure
> - Adaptation to your specific environment and LLM APIs

## Models

The following LLMs were explored during the development and their results were compared to human coded transcripts:

- `GPT-4`
- `Mistral`
- `Meta LLaMA`
- `DeepSeek Coder`

Other models can be integrated by modifying the prompt formatting and API wrappers.

### Resuluts

The results...

## Structure

llm-thematic-analysis/

│

├── README.md

├── Schema_Prompt_Overview_for_GitHub.ipynb  

## Contact

For questions or suggestions, feel free to open an issue or contact me directly.

