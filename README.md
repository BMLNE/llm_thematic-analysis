# Hybrid LLM-Based Thematic Analysis Pipeline

This repository presents a modular pipeline for conducting inductive and hybrid thematic analysis using a pre-trained LLMs. 
The project was developed as part of my Master’s thesis in the "Applied Data Information & Science" program at Lucerne University of Applied Sciences and Arts (HSLU). The aim of the thesis is to explore the capabilities and limitations of LLMs in automating qualitative research with Thematic Analysis (TA).


## Abstract (Master Thesis)
This thesis proposes and assesses a modular Large Language Model (LLM)-based pipeline for the automated thematic analysis of qualitative textual feedback from audio, developed in collaboration with the Swiss startup Voicy AG. The pipeline addresses the need for scalable, explainable, and efficient analysis tools by supporting four key steps: quote extraction, inductive code generation, semantic clustering, and theme abstraction. The proposed methodology is applied to a real-world dataset of transcribed German voice messages and evaluated using a human-coded reference as benchmark.
In order to assess the performance of the model, the pipeline is implemented and tested across three state-of-the-art LLMs: OpenAI, Mistral, and Llama. The findings demonstrate that open-source models, particularly Mistral, are capable of reliably performing early-stage tasks such as quote identification and inductive coding. These models generate semantically coherent codes that frequently correspond with human annotations, albeit at a more abstract level. It is evident that performance undergoes a further enhancement when evaluated semantically as opposed to structurally. However, all models encounter difficulties with theme synthesis, particularly when aligning quotes, codes, and abstract, human-defined themes.
Despite these limitations, the pipeline achieves significant gains in efficiency and adaptability. With runtimes under one hour and minimal resource requirements, it enables scalable qualitative analysis in time-sensitive and resource-constrained settings. Its parameterized architecture allows adaptation to different analytical needs, making it suitable for exploratory studies or hybrid human–AI workflows. While LLMs cannot yet replace human interpretive depth, they offer a strong foundation for assistive, transparent, and scalable qualitative analysis.

Keywords: thematic analysis, large language models, qualitative feedback, automated coding, explainable AI

## Context

TA is a powerful qualitative method for identifying and interpreting patterns in text data. However, it is labor-intensive and difficult to scale. This project explores how pre-trained LLMs can support or automate TA workflows.

1. Quote-level initial coding
2. Semantic clustering of codes
3. Hybrid codebook generation
4. Theme synthesis

### References 

It builds upon recent academic foundations:

- **Raza et al. (2025)** – *LLM-TA: An LLM-Enhanced Thematic Analysis Pipeline for Transcripts from Parents of Children with Congenital Heart Disease*
- **Katz et al. (2024)** – *Thematic Analysis with Open-Source Generative AI and Machine Learning: A New Method for Inductive Qualitative Codebook Development*
- **De Paoli (2024)** – *Performing an Inductive Thematic Analysis of Semi-Structured Interviews With a Large Language Model: An Exploration and Provocation on the Limits of the Approach*

## Overview

The notebook `01_LLM-Pipeline_Schema-Prompt-Design.ipynb` illustrates a simplified and modular version of a thematic analysis workflow. It highlights key steps such as:

- Text/transcript chunking and preparation
- Prompting strategies for different stages (code generation, theme abstraction)
- NLP components like embedding and clustering approaches

> Note: This notebook is a research prototype. It requires:
> - Manual loading of your own textual data and its structure
> - Adaptation to your specific environment and LLM APIs
> - Adjustments to your specific use case

The notebook `02_LLM-Human_Comparison_Evaluation.ipynb` provides a performance benchmark comparing LLM outputs to human-coded results.

### Repository Structure

llm-thematic-analysis/

> │
> 
> ├── `01_LLM-Pipeline_Schema-Prompt-Design.ipynb`   # Prompting design & pipeline logic
> 
> ├── `02_LLM-Human_Comparison_Evaluation.ipynb`       # Evaluation of LLM results against human coding
> 
> ├── `README.md`


## Conclusion of the Master Thesis
This study developed and evaluated a modular, LLM-based pipeline for automated thematic analysis of qualitative feedback. The results demonstrate that pre-trained LLMs, particularly Mistral, can reliably perform early TA stages like quote extraction and inductive coding, generating semantically meaningful codes aligned with human references.

Key insights:
- Structural precision is limited, but semantic alignment is strong.
- Theme abstraction remains a key weakness.
- All models underperform in aligning quote–code–theme relationships.

Despite these challenges, the pipeline:
- Operates with minimal computational requirements
- Finishes processing in under an hour
- May scales across datasets and contexts
- Supports parameterized, transparent analysis

LLMs are not yet a substitute for human insight but serve as powerful assistants in hybrid workflows. This pipeline marks a promising step toward scalable, explainable, and semi-automated qualitative research.


## Contact

For questions, feedback, or collaboration ideas, feel free to open an issue or contact me directly.
