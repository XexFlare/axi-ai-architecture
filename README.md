# Axi AI Architecture

Axi AI is a self-hosted AI inference ecosystem backed by Microsoft Phi designed to provide a centralized LLM API powering multiple independent applications.

## 🧠 Overview

The system separates AI inference from application logic:

- AI VPS → runs LLM inference
- App VPS → runs business logic, RAG, and UI layers

This design enables:
- reuse of a single AI backend
- improved cost efficiency
- modular application development

---

## 🏗️ Architecture


[ Applications Internal ]
├── Chat UI
├── Aphrodite (Personality Layer)
[ Applications External ]
├── Africa AI News Xpo
└── Corporate Policy RAG AI Xpo
└── Corporate Logisitcs AI Xpo
↓
API.AxiAI.site
↓
[ AI Inference Server {Docker Containerized} ]
└── Quantized LLM (Microsoft Phi / LLaMA via llama.cpp)


---

## 🔌 Core Components

| Component | Description |
|----------|------------|
| Inference Server | Runs the LLM and handles generation |
| API Layer | Secure access point for all applications |
| Chat UI | Standard conversational AI interface |
| Aphrodite | Personality-driven AI interface |

---

## 🎯 Goals

- Eliminate reliance on external AI APIs
- Enable private, controllable AI systems
- Provide a unified intelligence layer for multiple apps

---

## 📦 Repositories

- Inference Server → https://github.com/yourname/axi-ai-inference-server
- Chat UI → https://github.com/yourname/axi-ai-chat
- Aphrodite → https://github.com/yourname/axi-ai-aphrodite
- Website → https://github.com/yourname/axi-ai

---

## 🚀 Status

In active development.
