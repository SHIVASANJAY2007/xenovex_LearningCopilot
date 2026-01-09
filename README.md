# ⚡ XENOVEX: Personalized Learning Copilot

<p align="center">
  <img src="https://img.shields.io/badge/n8n-Workflow-FF6C37?style=for-the-badge&logo=n8n&logoColor=white" />
  <img src="https://img.shields.io/badge/AI-Agentic-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/RAG-Enabled-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" />
</p>



**XENOVEX** is an intelligent, agentic study assistant designed to bridge the gap between "dense course material" and "effective learning." Unlike generic AI, XENOVEX uses **Retrieval-Augmented Generation (RAG)** to ensure every answer is grounded in your specific textbooks and syllabus.

---

## 💎 Features & Capabilities

| Feature | Description |
| :--- | :--- |
| **🎯 Goal-Oriented RAG** | Answers questions using *only* your uploaded PDFs with full citations. |
| **🗓️ Dynamic Planner** | Converts syllabi into realistic weekly study schedules based on your free time. |
| **🧠 Adaptive Memory** | Tracks topic-wise proficiency (Low/Med/High) to prioritize weak areas. |
| **🔧 Tool Orchestration** | Powered by n8n workflows for transparent, logic-based decision making. |
| **🔒 Privacy First** | Minimal data footprint; supports local LLM integration for maximum security. |

---

## 🛠️ Tech Stack

* **Orchestration:** [n8n](https://n8n.io/) (Agentic Workflows)
* **LLM Support:** OpenAI GPT-4 / Anthropic Claude / Ollama (Local)
* **Vector Engine:** Pinecone / Supabase Vector (for course retrieval)
* **Storage:** Postgres / n8n Binary Store (for memory & session state)
* **Interface:** n8n Chat Trigger / Webhook-based UI

---

## 🚀 Getting Started

### 1. Installation
Clone this repository to access the workflow JSON files:
```bash
git clone [https://github.com/yourusername/xenovex.git](https://github.com/yourusername/xenovex.git)
cd xenovex
