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

# DecoBot 🤖 | Rule-Based AI Chatbot

[![Batch](https://img.shields.io/badge/Batch-2026-blue.svg)](https://github.com/)
[![Project Milestone](https://img.shields.io/badge/Project-1-green.svg)](https://github.com/)
[![Platform](https://img.shields.io/badge/Platform-DecodeLabs-orange.svg)](https://www.decodelabs.tech/)

An elegant, deterministic chatbot built from pure standard-library Python. Developed as part of the **DecodeLabs AI Engineering Milestone 1**, this project implements a rigid logic framework mimicking real-world AI guardrail systems.

---

## 🏗️ Architectural Phases Explained

This chatbot operates on a strict **Input ➔ Process ➔ Output (IPO)** system blueprint. Below is the engineering breakdown of why each structural phase is vital to the application.



### 🧠 PHASE 1 ── KNOWLEDGE BASE (Hash-Map / Dictionary)
* **The System's Core Brain:** Because rule-based systems do not possess probabilistic learning models, they rely entirely on pre-seeded human intent patterns. 
* **Optimized Lookup Performance ($O(1)$):** Using a Python dictionary allows the logic engine to evaluate intents instantly. This approach completely bypasses the computational and maintenance mess of traditional, deeply nested `if-elif` control ladders.

### 🧼 PHASE 2 ── SANITIZATION ENGINE
* **Normalizing Human Friction:** Real-world users introduce high noise into terminal inputs through irregular spacing, panicked punctuation (`!!`), and random case shifts (`HeLlO?`).
* **Determinism Safety:** The sanitization pipeline strips trailing punctuation, forces strings to lowercase, and collapses internal whitespace gaps. This guarantees that incoming noisy user data translates perfectly into structured keys that the system can recognize.

### 🩻 PHASE 3 ── INTENT MATCHING ENGINE (The Logic Skeleton)
* **Tiered Routing Strategy:** This layer functions as the decision gatekeeper. It processes matches down a rigid fallback chain: **Tier 0** checks for immediate exit kill-signals, **Tier 1** processes lightning-fast exact dictionary matches, and **Tier 2** falls back to keyword-in-string partial tracking.
* **Graceful Degradation:** When an unknown string bypasses exact or partial matches, **Tier 3** safely triggers a non-breaking fallback response. This prevents runtime system crashes while managing user expectations transparently.

### 🖨️ PHASE 4 ── OUTPUT ENGINE (Pretty Printing)
* **User Experience (UX) Emulation:** Dumping text instantly onto a command line feels sterile and unengaging. This phase introduces artificial millisecond delays between characters to cleanly simulate a live terminal "typing" response.
* **Visual Separation:** Handles structural formatting, initialization banners, and speaker tags (`👤 You:` vs `🤖 DecoBot:`) to maintain clean scannability inside the interface.

### 💓 PHASE 5 ── THE MAIN LOOP (The Heartbeat)
* **Persistent Runtime Lifecycle:** Script execution naturally halts once its code rows finish interpreting. The infinite `while True` loop serves as the heartbeat, constantly keeping the application alive and listening for new inputs.
* **Orchestration & State Management:** This layer synchronizes the execution flow—waiting on inputs, feeding them into the sanitization pipeline, evaluating matching tiers, counting total user exchanges, and handling graceful, non-corrupting user session terminations.

---

## 🛠️ Tech Stack & Requirements

* **Language:** Python 3.x
* **Libraries:** `time`, `random` (Strictly Python Standard Library—no external dependencies required)
* **Model Type:** Deterministic Rule-Based System / Non-Probabilistic

---
**📸 Output Screenshot**
<img width="1672" height="585" alt="ai_chatbot" src="https://github.com/user-attachments/assets/ff33916f-2fa8-41e4-bb71-1d422a741e63" />


## 🚀 Execution Summary Reference

```text
────────────────────────────────────────────────────────────
          DecodeLabs | Batch 2026 | Project 1
            RULE-BASED AI CHATBOT  🤖

       Type 'help' to see what I know.
       Type 'exit' to shut me down.
────────────────────────────────────────────────────────────
    
🤖 DecoBot: Hello! I'm DecoBot, your DecodeLabs AI assistant. How can I help you today?
────────────────────────────────────────────────────────────

👤 You: what is python
🤖 DecoBot: Python is the language I'm written in! It's powerful, readable, and has amazing libraries for AI.


