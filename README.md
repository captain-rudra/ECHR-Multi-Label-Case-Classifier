# ECHR Multi-Label Case Classifier

## Overview
This project implements a multi-label classification model using **LegalBERT** to predict which articles of the European Convention on Human Rights (ECHR) are relevant to a given legal case based on its factual description.

## Dataset
- **Source**: [LexGLUE – ECTHR-B](https://huggingface.co/datasets/lex_glue)
- **Description**: Approximately 11,000 legal case facts with associated ECHR articles.
- **Task**: Multi-label classification.

## Approach
1. **Data Preprocessing**: Tokenization, multi-hot label encoding, and dataset splitting.
2. **Model**: LegalBERT with a linear classifier head.
3. **Training**: Fine-tuning using AdamW optimizer with a learning rate of 2e-5.
4. **Evaluation**: Metrics include Micro-F1, Macro-F1, and Hamming Loss.

## Results
![Evaluation Metrics](eval.png)

## Usage
1. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
