# Dataset

This folder contains the benchmark dataset for **FrameNet-Cultures: A Benchmark for Evaluating LLMs via Cross-Cultural Frame Semantics**.

## Contents

This directory includes:

- 18 frame-specific CSV files.
- Ethnographic (gold) cultural representations extracted from the EveryCulture encyclopedia.
- LLM-generated cultural descriptions.
- Binary feature annotations for both the gold and LLM-generated data.
- CSV files containing the generated dialogues used in the human evaluation experiments.

The prompt templates used to generate the model outputs are available in the `prompts/` directory, including:

- Culture-neutral prompts
- Culture-specific prompts aligned with India
- Culture-specific prompts aligned with Ethiopia
- Dialogue-generation prompts used for the human evaluation experiments

For details about the benchmark construction, annotation guidelines, and evaluation protocol, please refer to the accompanying paper and the main repository README.
