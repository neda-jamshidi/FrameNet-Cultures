# FrameNet-Cultures

<div align="center">

#  FrameNet-Cultures
### A Benchmark for Evaluating Large Language Models via Cross-Cultural Frame Semantics

**Findings of ACL 2026**

**Neda Jamshidi<sup>1,2</sup>, Anders Søgaard<sup>1</sup>, Monica Bianchini<sup>2</sup>**

<sup>1</sup>University of Copenhagen, Denmark  
<sup>2</sup>University of Siena, Italy

📄 **Paper:** *FrameNet-Cultures: A Benchmark for Evaluating LLMs via Cross-Cultural Frame Semantics*

</div>

---

## Overview

Large Language Models (LLMs) generate culturally rich content about everyday social practices such as greetings, food, marriage, religion, and family life. However, existing cultural evaluation benchmarks primarily rely on closed-form multiple-choice questions or predefined cultural dimensions, making it difficult to assess whether models genuinely capture cultural knowledge or simply memorize common stereotypes.

**FrameNet-Cultures** is the **first open-ended benchmark** that evaluates the cultural alignment of LLMs using **Frame Semantics**. Instead of asking models factual questions, our benchmark measures how models instantiate culturally grounded semantic frames and compares these representations with human-authored ethnographic knowledge.

The benchmark is constructed from the **EveryCulture** encyclopedia and provides an interpretable framework for studying cultural bias, cultural alignment, cultural homogenization, and cultural adaptability in modern LLMs.

---

## ✨ Highlights

- **20 countries** spanning five continents
- **18 cultural semantic frames**
- Human-authored ethnographic reference data
- Evaluation of **5 state-of-the-art LLMs**
- Open-ended cultural generation
- Binary cultural feature annotations
- Quantitative evaluation using Normalized Hamming Distance
- PCA visualization of cultural representations
- Human evaluation of cultural recognizability
- Fully open benchmark

---

## Cultural Frames

The benchmark covers 18 culturally grounded semantic frames:

- Food
- Greeting
- Marriage
- Religion
- Secular Celebrations
- Symbolism
- Ethnic Relations
- Government
- Classes and Castes
- Gender Roles and Status
- Domestic Units
- Kin Groups
- Inheritance
- Child Rearing
- Infants
- Higher Education
- Military Activity
- Death

---

## Countries

The benchmark includes cultural knowledge from the following countries:

- Australia
- Brazil
- China
- Denmark
- Egypt
- Ethiopia
- France
- Georgia
- Germany
- India
- Iran
- Italy
- Japan
- Mexico
- New Zealand
- Nigeria
- Russia
- Saudi Arabia
- Turkey
- United States

---

## Repository Structure

```text
FrameNet-Cultures/
│
├── data/
│   ├── Food.csv
│   ├── Greeting.csv
│   ├── Marriage.csv
│   ├── Religion.csv
│   └── ...
│
├── prompts/
│   ├── culture-neutral/
│   ├── india-alignment/
│   └── ethiopia-alignment/
│
├── annotations/
│
├── evaluation/
│
├── figures/
│
├── LICENSE
├── README.md
└── requirements.txt
```

---

## Dataset

Each cultural frame is represented as a CSV file.

Each instance contains culturally grounded semantic features extracted from ethnographic descriptions.

Example:

| Column | Description |
|----------|-------------|
| Country | Country associated with the cultural practice |
| Frame | Semantic frame |
| Feature | Cultural feature |
| Value | Binary annotation (0 or 1) |
| Description | Human-authored ethnographic evidence |

---

## Evaluation Tasks

FrameNet-Cultures supports multiple research tasks, including:

- Cultural Alignment
- Cross-Cultural Reasoning
- Open-ended Cultural Generation
- Cultural Bias Analysis
- Cultural Adaptation
- Frame Semantic Understanding
- Cross-Cultural Comparison
- Prompt-based Cultural Steering

---

## Evaluated Models

The benchmark is model-agnostic and can be used with any LLM.

The paper evaluates:

- ChatGPT-5
- Gemini 2.5 Flash
- Mistral Large
- Qwen-3 Max
- DeepSeek V3.2

---

## Evaluation Metrics

FrameNet-Cultures evaluates generated cultural representations using:

- Normalized Hamming Distance
- Country-level Alignment
- Continent-level Alignment
- Frame-level Alignment
- Principal Component Analysis (PCA)
- Human Evaluation

---

## Main Findings

Our experiments reveal several consistent patterns across state-of-the-art LLMs:

- LLMs exhibit a strong **Europe-centered cultural bias** under culture-neutral prompting.
- Cultural representations become increasingly **homogenized** across different countries.
- Explicit cultural conditioning shifts model representations toward target cultures but does not fully recover ethnographic cultural structures.
- Structured prompting substantially improves the human recognizability of generated cultural content.

---

## Citation

If you use **FrameNet-Cultures** in your research, please cite:

```bibtex
@inproceedings{jamshidi2026framenetcultures,
  title={FrameNet-Cultures: A Benchmark for Evaluating LLMs via Cross-Cultural Frame Semantics},
  author={Jamshidi, Neda and Søgaard, Anders and Bianchini, Monica},
  booktitle={Findings of the Association for Computational Linguistics: ACL 2026},
  year={2026}
}
```

---

## License

This dataset is released for **research and educational purposes**.

Please refer to the **LICENSE** file for details.

---

## Contact

**Neda Jamshidi**

PhD Candidate in Artificial Intelligence  
Department of Information Engineering and Mathematical Sciences  
University of Siena, Italy

Visiting Researcher  
Natural Language Processing Group  
University of Copenhagen, Denmark

📧 **Email:** neda.jamshidi@student.unisi.it

---

## Acknowledgements

This work was conducted through the collaboration between the **University of Siena** and the **University of Copenhagen**.

We thank the native annotators and the contributors who participated in the human evaluation of the benchmark.

---

⭐ **If you find this benchmark useful, please consider starring the repository!**
