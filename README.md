# multi-agent-article-writer-crewai# Multi-Agent Article Writer with CrewAI

This project demonstrates how to build a simple **multi-agent AI workflow** using **CrewAI** to research, plan, write, and edit an article automatically.

The notebook creates a small team of AI agents that collaborate in sequence:

- **Content Planner** – researches the topic and creates a structured content plan
- **Content Writer** – writes the article based on the plan
- **Editor** – revises the article for clarity, grammar, and tone

## Project Overview

The main goal of this project is to show how **multi-agent systems** can be used to break a writing task into specialized steps. Instead of asking one model to do everything, different agents handle different responsibilities.

This notebook includes:

- Agent creation with roles, goals, and backstories
- Task design for planning, writing, and editing
- Crew creation and execution using CrewAI
- Example run on the topic **Artificial Intelligence**
- A section for trying your own custom topic

## Workflow

The system follows this pipeline:

1. **Plan** the article content
2. **Write** the article draft
3. **Edit** the final output

Because the tasks are sequential, each step depends on the result of the previous one.

## Technologies Used

- Python
- [CrewAI](https://github.com/joaomdmoura/crewAI)
- crewai_tools
- langchain_community
- OpenAI GPT model (`gpt-3.5-turbo` in the notebook)
- Jupyter Notebook

## File

- `L2_research_write_article.ipynb` – main notebook containing the full implementation

## Installation

If you are running this locally, install the required packages:

```bash
pip install crewai==0.28.8 crewai_tools==0.1.6 langchain_community==0.0.29
