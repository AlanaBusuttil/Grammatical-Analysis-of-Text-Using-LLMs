# Grammatical Inference of Maltese Words Using Neural Networks

## Overview

This project investigates **grammatical inference** of Maltese words, with a specific focus on **morphological analysis**. Maltese is a hybrid language with deep **Semitic influences**, particularly evident in its grammar. Due to this complexity, the project approaches grammatical inference from both **monolingual** and **multilingual** perspectives.

Given that Maltese is a **low-resource language**—with limited human-annotated data for grammatical analysis—this project explores **neural network-based methods** to perform morphological parsing. The aim is to develop models that take a **Maltese word as input** and output its **full grammatical analysis**.

## Dataset

The dataset used for training and evaluation is adapted from **[UniMorph](https://unimorph.github.io/)**, a universal morphological annotation project. The Maltese portion was curated and processed to suit the input-output requirements of neural network training.

## Objectives

- Develop and evaluate computational models for morphological analysis of Maltese.
- Compare **baseline RNN models** with **pre-trained transformer-based models**.
- Investigate the impact of **cross-lingual transfer** and **domain-specific fine-tuning** on model performance.
- Evaluate the utility of **monolingual vs multilingual** models in the context of a hybrid, low-resource language.

## Models and Methodology

### Baseline Model

- **Recurrent Neural Network (RNN)**: Built from scratch and trained directly on the Maltese morphological dataset. Acts as the performance baseline.

### Pre-trained Models

#### General Pre-trained Models
- **BERT (English)**: A monolingual model pre-trained on English.
- **mBERT**: A multilingual model trained on 104 languages.

#### Maltese-Specific Pre-trained Models
- **BERTu**: A monolingual Maltese language model further pre-trained on Maltese corpora.
- **mBERTu**: A multilingual model (based on mBERT) further pre-trained with additional Maltese data.

## Experimental Notebooks

### Comparative Models for Grammatical Analysis

| Model Type          | Notebook File                      |
|---------------------|------------------------------------|
| BERT (English)      | `BERT_english_model.ipynb`         |
| BERT (Italian)      | `BERT_italian_model.ipynb`         |
| BERTu (Maltese)     | `BERT_U_model.ipynb`               |
| mBERTu (Maltese)    | `mBERT_u_model.ipynb`              |

### Cross-Lingual and Zero-Shot Tests

| Experiment                                | Notebook File                                |
|-------------------------------------------|----------------------------------------------|
| mBERTu with cross-lingual transfer        | `mBERT_U_with_crosslingual_transfer.ipynb`   |
| BERTu with zero-shot evaluation           | `BERT_U_model_with_zero_shot.ipynb`          |

## Results and Findings

The final evaluation compared the performance of all models on grammatical inference tasks. Results showed that **Maltese-specific pre-trained models significantly outperformed** the general-purpose BERT models.

- The **mBERTu** model achieved the highest performance across all evaluation metrics.
- The findings highlight the importance of **language-specific pre-training** for low-resource languages with unique linguistic structures.

## Contribution and Significance

This is the **first project to apply neural networks for grammatical inference in the Maltese language**. It contributes to ongoing efforts in NLP for under-resourced languages by:

- Introducing and evaluating neural approaches for Maltese morphology.
- Demonstrating the effectiveness of transfer learning and domain-specific pre-training.
- Laying the groundwork for future research in Maltese NLP applications.

link to study: https://www.um.edu.mt/library/oar/handle/123456789/115279
