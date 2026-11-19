# CatalystBench

CatalystBench evaluates language models on eight tasks in catalysis science. This repository contains **4,037 evaluation examples**, with per-task from the paper’s 15% test-set protocol.

[ICLR 2026 Paper](https://proceedings.iclr.cc/paper_files/paper/2026/hash/3449f32354933cd6f063112897c406f2-Abstract-Conference.html) · [PDF](https://proceedings.iclr.cc/paper_files/paper/2026/file/3449f32354933cd6f063112897c406f2-Paper-Conference.pdf)

| Task | File | Examples |
|---|---|---:|
| Regulation Scheme Comprehension | [RSC.jsonl](RSC.jsonl) | 646 |
| Material Extraction | [ME.jsonl](ME.jsonl) | 372 |
| Regulation Method Classification | [RMC.jsonl](RMC.jsonl) | 355 |
| Synthesis Extraction | [SE.jsonl](SE.jsonl) | 992 |
| Faradaic Efficiency Prediction | [FEP.jsonl](FEP.jsonl) | 322 |
| Formation Energy Prediction | [FP.jsonl](FP.jsonl) | 450 |
| d-band Center Prediction | [d-CP.jsonl](d-CP.jsonl) | 450 |
| Adsorption Energy Prediction | [AP.jsonl](AP.jsonl) | 450 |
| **Total** | | **4,037** |

Each JSONL line contains one example. Use `instruction` and `input` as the model prompt, and `output` as the reference answer. Additional fields provide identifiers, source information, and multi-turn annotations where applicable. Samples were selected and constructed from annotated corpora and public datasets. Numerical targets use **%** for FEP, **eV/atom** for FP, and **eV** for AP and d-CP. d-band centers are referenced to the Fermi level. For task definitions, data construction, and prompt templates, see **Appendix A**, **Section 5.1**, and **Appendix D** of the paper.
