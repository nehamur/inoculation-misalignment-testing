# Inoculation Prompting and Emergent Misalignment
### Neha Muramalla and Reshma Kosaraju

This repository contains the report for the MIT 6.7960 Deep Learning final project:

**Does Inoculation Prompting Remove or Mask Emergent Misalignment?  
A Representation-Level Study Using Persona Vectors**

We study whether inoculation prompting (IP), a proposed defense against emergent misalignment (EM), genuinely removes misaligned representations or merely suppresses their surface expression.

Our results reveal a dissociation between representation-level alignment metrics and behavioral robustness under adversarial attack.

---

## 🔍 Key Findings

- **Inoculation prompting increases vulnerability** to jailbreak attacks, especially for otherwise well-aligned models.
- **Persona vector projections suggest improved alignment**, but behavioral evaluations show the opposite.
- IP creates **stronger, more distinct persona representations in orthogonal space**, rather than removing misaligned structure.
- Representation-level alignment does **not guarantee behavioral robustness**.

---

## 🧠 Methods Overview

- **Models:** Qwen2.5-Coder-7B-Instruct
- **Training conditions:** CLEAN, EM, CLEAN+IP, EM+IP (2×2 design)
- **Representation analysis:** Persona vectors (difference-in-means over residual stream activations)
- **Behavioral evaluation:** Automated jailbreak testing on AdvBench and HarmBench
- **Judging:** LLM-as-a-judge with confidence filtering

---

## 📄 Interactive Report

The full paper is available as a static HTML page:

👉 **[View the report](https://nehamur.github.io/inoculation-misalignment-testing/)**

(Hosted via GitHub Pages.)

---

## 📁 Repository Structure

```text
.
├── index.html              # Main paper (static HTML)
├── blog_files/             # Figures and plots
├── README.md
└── assets/ (optional)      # Additional resources
