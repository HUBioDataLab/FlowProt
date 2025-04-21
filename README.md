
# FlowProt

**FlowProt: Classifier-Guided Flow Matching for Targeted Protein Backbone Generation in the de
novo DNA Methyltransfarase Family**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Model Type](https://img.shields.io/badge/model-flow--matching-lightgrey)]()

---

## Overview

**FlowProt** is a flow-matching generative model guided by a domain classifier for the **targeted generation of protein backbones**, demonstrated on the **de novo DNA methyltransferase (DNMT) family**.

> FlowProt is a **method combining flow matching with classifier guidance** for functional protein design.

- Generates **structurally stable and functionally targeted** protein backbones
- Guided using classifier feedback to focus on **DNMT-like** domains
- Built on the [FrameFlow](https://arxiv.org/abs/2310.05297) architecture

---

## Repository Structure
Work in progress..

---

## Method Summary

<p align="center">
  <img src="figures/inference_diagram.png" width="600">
</p>

1. Start from random noise  
2. Predict backbone transformations (rotation + translation)  
3. Classifier guides each step toward **DNMT3A-like** structures  
4. Evaluate quality & function (ProteinMPNN → ESMFold → ProGReS)

---

## Results Summary

| Sequence Length | scRMSD ↓ | scTM ↑ | pLDDT ↑ | progres ↑ |
|------------------|----------|--------|----------|------------|
| 286 (DNMT3A)     | 3.10     | 0.86   | 83.12    | 0.53       |

> FlowProt performs best in the mid-length range and excels at 286 residues—the exact length of human DNMT3A.

---

## Installation

Work in progress...

---

## Training & Inference

Work in progress...

---

## Contact

Feel free to open an issue or reach out:  
📧 alibaran [at] tasdemir.us

---

## Acknowledgements

- FrameFlow (Yim et al. 2023)  
- ESMFold, ProteinMPNN, and progres authors
