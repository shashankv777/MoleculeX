# MoleculeX: AI-Powered Genomic Mutation Analyzer

MoleculeX is an advanced AI-driven platform that predicts the pathogenicity of genomic mutations—especially single nucleotide variants (SNVs)—to aid in early disease detection and drug research. Leveraging large language models like Evo2, the platform empowers researchers and bioinformaticians to analyze, interpret, and visualize human DNA sequences with high precision.

## Project Highlights

- Uses Evo2 LLM, trained on ~3 trillion base pairs, to classify SNVs.
- Achieves ~0.92 AUROC on BRCA1 benchmark dataset (LOF vs FUNC/INT).
- Pulls data from ClinVar and UCSC Genome Browser to enrich predictions.
- Provides an interactive dashboard for genomic variant analysis and visualization.
- Deploys scalable inference using Modal on H100 GPUs.

## Use Case

MoleculeX helps researchers and biotech companies:

- Predict whether a genetic mutation is likely to cause disease (pathogenic).
- Automate analysis pipelines for variant classification.
- Integrate large language models into genomic workflows.
- Support AI-driven drug discovery pipelines.

## Evo2 Model Integration

- Evo2 is a foundation model for DNA, trained on public genomic corpora.
- In MoleculeX, it is used to compute "delta scores": a signal for pathogenicity based on sequence context.
- Achieved 0.92 AUROC on BRCA1 SNVs, outperforming traditional scoring methods.

## Tech Stack

Frontend: Next.js, React, TypeScript  
Backend: FastAPI  
Inference: Evo2 LLM via Modal (H100 GPUs)  
Database: ClinVar, UCSC Genome Browser (API-integrated)  
Deployment: Modal.com (Cloud GPU inference)  
Authentication (Planned): Firebase or Auth.js  

## APIs and Datasets

- ClinVar API: Fetches known SNV clinical interpretations.
- UCSC Genome Browser API: Annotates mutations with genomic context.
- BRCA1 Benchmark Dataset: Used for evaluation and validation.


