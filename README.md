# ⚡ XENOVEX: Personalized Learning Copilot
> **Stage:** v0.1-Alpha (Initial Release)
> **Engine:** n8n Agentic Workflow

XENOVEX is a lightweight AI-driven study tool designed to solve student organization and study efficiency problems. Built entirely within **n8n**, it moves beyond a simple chatbot by implementing a structured agentic workflow to handle academic materials.

<p align="left">
  <img src="https://img.shields.io/badge/n8n-Workflow-FF6C37?style=for-the-badge&logo=n8n&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Initial_Prototype-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/AI-Agentic_RAG-blueviolet?style=for-the-badge" />
</p>

---

## 🏗️ Project Architecture (Initial Stage)

Currently, XENOVEX operates as a **Working AI Agent** within n8n. Instead of a "black-box" prompt, the logic is broken down into modular steps:

* **The Orchestrator:** n8n manages the flow, deciding when to retrieve data and when to respond.
* **The Brain:** LLM (OpenAI/Claude) connected via the AI Agent node.
* **Knowledge Base:** RAG-ready structure for Syllabus and Notes ingestion.
* **Context Management:** Chat history and lightweight memory storage.

---

## 🚀 Current Roadmap

| Phase | Description | Status |
| :--- | :--- | :---: |
| **Phase 1** | Core n8n AI Agent Setup (ChatGPT-like logic) | ✅ Done |
| **Phase 2** | Vector Store Integration (Course RAG) | 🏗️ In Progress |
| **Phase 3** | Automated Study Planner Node | 📅 Planned |
| **Phase 4** | Dashboard / Simple Web UI | 📅 Planned |

---

## 🛠️ Setup Instructions

To get this "Initial Stage" agent running in your own n8n instance:

### 1. Requirements
* An **n8n** instance (Desktop or Docker)
* An **OpenAI API Key** (for the Agent node)
* (Optional) **Ollama** for local inference

### 2. Import Workflow
1. Download the `xenovex_v1_agent.json` from the `workflows/` folder.
2. In n8n, click **Workflows** > **Import from File**.
3. Connect your **AI Agent** node to your OpenAI/Local LLM credentials.

### 3. Test the Agent
* Use the **Chat Window** within n8n to interact.
* The current agent is configured to recognize academic queries and maintain conversation memory.

---

## 🧬 How it Works (The Workflow)

```mermaid
graph TD
    A[User Query] --> B{n8n Orchestrator}
    B --> C[AI Agent Node]
    C --> D[Chat Memory]
    C --> E[Vector Store/Tools]
    E --> F[Contextual Response]
    F --> G[Final User Answer]
