# 🧠 AI Research Assistant

## 🚀 Overview

**AI Research Assistant** is a Python-based intelligent automation system designed to streamline the **research process** using multiple coordinated **AI agents**.  
Each agent is specialized — one performs research, another analyzes data, and another writes content — all working together to produce high-quality research outputs efficiently.

This project leverages **CrewAI** to manage and orchestrate collaboration among agents, ensuring that complex research workflows can be automated and extended easily.

---

## 📘 Table of Contents

1. [Overview](#-overview)  
2. [Repository Structure](#-repository-structure)  
3. [Installation & Setup](#-installation--setup)  
4. [How It Works](#-how-it-works)  
5. [Features](#-features)  
6. [Usage Examples](#-usage-examples)  
7. [Extending / Contributing](#-extending--contributing)  
8. [Dependencies](#-dependencies)  
9. [License](#-license)  
10. [Contact](#-contact)

---

## 📂 Repository Structure


**Key Directories:**

- **`agents/`** — Contains the specialized AI agent scripts.
- **`tasks/`** — Houses the task logic or helpers that the agents rely on.
- **`crew.py`** — Manages the interaction between agents.
- **`app.py`** — Main runner that coordinates workflow execution.
- **`env_template.txt`** — Template for environment variables (e.g., API keys).

---

## 🔧 Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/Adelakun1999/ai-research-assistant.git
cd ai-research-assistant

```

### 2. Create and activate a virtual environment

```
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install dependencies
```
pip install -r requirements.txt
```

### 4. Configure environment variables

Copy the template file and set your API keys or other secrets:
```
cp env_template.txt .env
```
Then open .env and fill in values such as:
```
OPENAI_API_KEY=your_api_key_here
SERPER_API_KEY=your_serper_key_here
```
### 5. Run the application
```
streamlit run app.py
```

**🧭 How It Works**
```
- Initialization:
The system loads environment variables and initializes the CrewAI environment.

- Agent Collaboration:
The Research Agent fetches or summarizes research material.
The Data Analysis Agent interprets key findings.
The Content Writer Agent composes structured blog posts, summaries, or articles.

- Workflow Coordination:
crew.py manages the pipeline — ensuring results from one agent are passed to the next.

- Final Output:
The output is a coherent research summary, report, or blog post, ready for publication or further refinement.

```

**🌟Features**

✅ Modular and extensible agent-based architecture

✅ Automated research and analysis pipeline

✅ Seamless coordination using CrewAI

✅ Environment-driven configuration

✅ Reusable and customizable for multiple use cases (research, blog generation, content creation)



