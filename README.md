# GenAI Language Architect: Multi-Agent Learning System

A modular, containerized platform designed to demonstrate the orchestration of Generative AI for structured language acquisition.  
This repository serves as a blueprint for building scalable, LLM-agnostic applications using modern architectural patterns.

---

## 🏗️ System Architecture

The system is built on a **Decoupled Micro-Service Architecture**, ensuring that the user interface, business logic, and LLM orchestration layers remain independent and scalable.

### Architectural Pillars

- **Provider Agnostic**  
  Built to switch seamlessly between Cloud LLMs (OpenAI, Claude) and Local LLMs (Ollama) using a standardized adapter pattern.

- **Container-First Orchestration**  
  Every component (Frontend, Backend, Database) is isolated via Docker, ensuring environment parity across development and production.

- **Prompt Engineering as a Service**  
  Centralized prompt management for specialized tasks like the *Sentence Constructor*, allowing iterative testing without redeploying core logic.

---

## 🛠️ Tech Stack

- **Frontend**: React / Next.js (Client-side state management and interactive UI)  
- **Backend**: Python Flask / FastAPI (RESTful API design and business logic)  
- **AI/ML**: OpenAI API, Ollama (Local inference), LangChain (Orchestration)  
- **Infrastructure**: Docker & Docker Compose (Containerization)

---

## 📂 Project Structure

| Component               | Description                          | Architectural Highlights                          |
|------------------------|--------------------------------------|--------------------------------------------------|
| `sentence-constructor/` | AI-powered grammar assistant         | Implements Chain-of-Thought prompting logic      |
| `language-portal/`      | Central management hub               | Demonstrates Service-Oriented Architecture (SOA) |
| `infrastructure/`       | Docker and deployment configurations | Ensures Infrastructure as Code (IaC) principles  |

---

## 🚀 Getting Started

### Prerequisites

- Docker & Docker Compose  
- Python 3.10+  
- API Keys for OpenAI 

### Installation

**Clone the repository:**
```bash
git clone https://github.com/emmaahmads/genai-language-architect.git
```
**Launch the environment:**
```bash
docker-compose up -d
```
## This project was developed as part of the Free GenAI Bootcamp 2025 to master the intersection of software architecture and Generative AI.
