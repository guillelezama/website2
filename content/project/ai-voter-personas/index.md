---
title: "AI Voter Personas: US 2024"
summary: Clustered 51 ANES policy variables into 15 voter segments and built a structured LLM interface grounded in empirical distributions. Includes a 10-question probabilistic assignment quiz and controlled prompting to prevent drift.
tags:
- python
- genai
- ml
date: "2025-01-15T00:00:00Z"

links:
- name: Live Demo
  url: https://anes-2024-personas.vercel.app/
- name: Code & Methodology
  url: https://github.com/guillelezama/anes-2024-personas

image:
  caption: ""
  focal_point: Smart
---

## Problem

How can we generate structured, data-grounded responses to new questions without fielding new surveys?

## Approach

- Variance-weighted K-means clustering (15 voter segments from 51 policy variables)
- Silhouette and stability diagnostics
- 10-question probabilistic assignment quiz
- Structured LLM conditioning grounded in cluster-level distributions
- Controlled prompting to prevent drift

## Validation

- Tested on 200 held-out ANES respondents
- Predictions meaningfully above chance
- Accuracy improved when demographics were included

## Limitations

- Smooths over individual inconsistency
- Augments but does not replace real surveys
