# Rule-Based AI Chatbot (DecoBot) 🤖

Welcome to **Project 1** for **DecodeLabs (Batch 2026)**. This project implements a deterministic, rule-based AI chatbot named **DecoBot** using pure Python. It serves as a foundational project to understand foundational logic control flow, exact/partial string matching architectures, and the classic **IPO (Input-Process-Output)** model before transitioning into probabilistic AI systems.

---

## 💡 What is Rule-Based AI?

A **Rule-Based AI** system relies on explicit, predefined rules to make decisions and generate responses. Unlike modern Machine Learning or Deep Learning architectures (like transformers or LLMs), it does not look for statistical patterns in historical datasets or dynamically infer meaning. 

### Key Characteristics:
* **Deterministic Logic:** The exact same input will consistently return the exact same output path. There is zero risk of "hallucination."
* **O(1) Efficiency:** Uses Hash-Maps (Python Dictionaries) for fast, near-instantaneous intent lookups.
* **White-Box Transparency:** Every single decision path can be completely traced, audited, and explained. It acts as the core foundational layer behind modern enterprise **AI Guardrails** (such as Nvidia NeMo or Llama Guard).

---

## 🏗️ Architectural Blueprint (The IPO Model)

DecoBot is engineered strictly around the standard computer science **Input ➔ Process ➔ Output (IPO)** model:
