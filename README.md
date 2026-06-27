# Rule-Based AI Chatbot (DecoBot) 🤖

Welcome to **Project 1** for **DecodeLabs (Batch 2026)**. This repository contains the complete implementation of **DecoBot**, a deterministic, rule-based AI assistant built entirely using Python's standard library. 

This project serves as an introductory milestone to master foundational computer science architectures, data structure lookups ($O(1)$ complexity), text standardization pipelines, and the classic **IPO (Input-Process-Output)** engineering loop before working with probabilistic machine learning networks.

---

## 👤 Project Credits
* **Author:** Mahidi Hasan Mithun
* **Platform:** DecodeLabs
* **Cohort:** Batch 2026
* **Milestone:** Project 1 (Rule-Based AI Chatbot)

---

## 💡 What is Rule-Based AI?

A **Rule-Based AI** system makes decisions and forms responses based on explicit, preconfigured rules established by the developer. It does not generalize or learn from patterns dynamically.

### Key Performance Profiles:
* **Deterministic Behavior:** The exact same user query yields the exact same logical execution path every time. There is **zero risk of hallucination**.
* **High Efficiency:** Uses memory-mapped Hash-Maps (Python `dict`), achieving $O(1)$ time complexity for immediate exact-match queries.
* **White-Box System:** Highly trace-auditable and explainable. This deterministic approach serves as the design architecture behind modern enterprise **AI Guardrails** (e.g., NVIDIA NeMo, Llama Guard) to filter toxic inputs before they reach LLMs.

---

## 🏗️ Architectural Blueprint: The IPO Model

The execution timeline follows a strict **Input ➔ Process ➔ Output** methodology:
