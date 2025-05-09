# Hybrid LLM-Based Thematic Analysis Pipeline

This repository presents a modular pipeline for conducting inductive and hybrid thematic analysis using a pre-trained LLMs. 
The project was developed as part of my Master’s thesis in the "Applied Data Information & Science" program at Lucerne University of Applied Sciences and Arts (HSLU). The aim of the thesis is to explore the capabilities and limitations of LLMs in automating qualitative research with Thematic Analysis (TA).


## Context

TA by Braun & Clarke (2006) is a powerful qualitative method for identifying and interpreting patterns in text data. However, it is labor-intensive and difficult to scale. This project explores how pre-trained LLMs can support or automate TA workflows.

1. Quote cxtraction & initial coding
2. Semantic clustering of initial codes
3. Hybrid codebook generation
4. Theme generation

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

## Abstract (Master Thesis)

This thesis proposes and assesses a modular Large Language Model (LLM)-based pipeline for the automated thematic analysis of qualitative textual feedback from audio, developed in collaboration with the Swiss startup Voicy. The pipeline is conceptually aligned with the six-phase approach to Thematic Analysis proposed by Braun & Clarke and addresses the need for efficient analysis tools by supporting four key steps: quote extraction, semantic clustering, inductive code generation, and theme abstraction. The proposed methodology is applied to a real-world dataset of transcribed German voice messages and evaluated using a human-coded reference as benchmark.
In order to assess the performance of the model, the pipeline is implemented and tested across three state-of-the-art LLMs: ChatGPT, Mistral, and Llama. The findings demonstrate that open-source models, particularly Mistral, are capable of reliably performing early-stage tasks such as relevant quote identification and inductive coding. The generated codes are semantically coherent and frequently align with human annotations, although they tend to operate at a higher level of abstraction and with less contextual nuance. However, all models face significant challenges in theme generation, particularly in synthesizing coherent, context-sensitive themes and consistently aligning them with the correct quotes and codes. These limitations underscore the need for improved abstraction strategies and better integration of contextual information.
Despite these limitations, the pipeline achieves significant gains in efficiency and adaptability. With runtimes under one hour and minimal resource requirements, it enables scalable qualitative analysis in time-sensitive and resource-constrained settings. Once the research design is defined, the pipeline can run in a fully automated manner. Its flexible, parameterized structure allows it to be adapted to a wide range of study types and analytical needs. While LLMs cannot yet replicate the interpretive depth of human analysts, they offer a strong foundation for scalable and assistive qualitative analysis. 

Keywords: thematic analysis, large language models, qualitative feedback, automated qualitative data analysis, inductive coding

## Conclusion of the Master Thesis

This study developed and evaluated a modular, LLM-based pipeline for conducting automated TA of qualitative feedback. The results demonstrate that pretrained LLMs, particularly open-source models like Mistral, are capable of reliably supporting the early stages of the TA process, such as quote extraction and hybrid code generation. The generated codes were semantically coherent and often aligned conceptually with human annotations, though they tended to operate at a higher level of abstraction and lacked fine-grained differentiation. However, the accurate assignment of codes to specific quotes or text segments remains inconsistent, indicating that the quote-level labeling is not yet fully reliable.
While quote-level extraction showed promising performance across all models, theme generation emerged as a major limitation. In general, the LLMs struggled to synthesize abstract, context-sensitive themes in ways that reflected the analytical framing of human coders. This limitation was particularly evident in the quote–code–theme alignment task, where structural mismatches persisted even under relaxed, semantic similarity conditions. Although code assignment at the quote level showed potential, the accuracy was not yet sufficient for applications requiring fine-grained interpretability.
Importantly, the pipeline was designed with automation, scalability, and explainability in mind. With runtimes under one hour and minimal computational cost, it presents a resource-efficient alternative to manual coding. The system architecture also enables parameterized input, making it adaptable to different use cases and scalable across large datasets. These features make LLM-based TA particularly attractive for exploratory research, time-sensitive evaluations, and resource-constrained environments, where approximate but interpretable insights can be highly valuable.
At the same time, the study highlights critical open challenges, including the need for improved theme abstraction, more precise quote–code alignment, human-in-the-loop design, and evaluation frameworks that better capture the conceptual nuances of qualitative data. While LLMs cannot yet replicate the interpretive depth of human analysts, they already provide a viable foundation for hybrid and assistive qualitative analysis workflows.


## Contact

For questions, feedback, or collaboration ideas, feel free to open an issue or contact me directly.
