# Technical Question Evaluation Across Language Forms

## Overview
An exploratory evaluation of Qwen/Qwen3-1.7B on technical questions
written in English, Roman Urdu, Urdu script, and code-switched language.

## Research question
Does the language form of a technical question affect the correctness
of model responses?

## Dataset
- 10 underlying technical questions
- 4 language forms per question
- 40 prompts in total
- Manual correctness scores on a 0–2 scale

## Preliminary results
| Language form | Mean correctness |
|---|---:|
| English | 1.8/2 |
| Code-switched | 1.8/2 |
| Roman Urdu | 1.4/2 |
| Urdu script | 1.5/2 |

These are exploratory results from a small pilot, not general claims
about model capabilities.

## Files
- `evaluation_dataset.csv`: Evaluation prompts
- `evaluation_results.csv`: Model responses
- `manual_scoring.csv`: Human evaluation scores and error notes
- `language_summary.csv`: Aggregate results
- `model_info.txt`: Model and experiment information
- `preliminary_findings.md`: Findings, limitations, and next steps

## Limitations
Only 10 underlying questions were evaluated. Translation equivalence,
topic coverage, decoding settings, and subjective scoring may affect
the results. Larger evaluations and independent reviewers are needed.

## Reproducibility
This repository contains evaluation artifacts, not model weights.
See `model_info.txt` for the recorded environment details.
