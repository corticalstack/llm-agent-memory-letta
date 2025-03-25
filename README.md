# 🧠 LLM Agent Memory with Letta

A hands-on course exploring the implementation and application of memory systems for Large Language Model (LLM) agents using the Letta framework.

## Description

This repository contains a series of Jupyter notebooks that guide you through building increasingly sophisticated memory systems for LLM agents. From implementing basic self-editing memory from scratch to orchestrating multiple agents with shared memory, this course provides a comprehensive exploration of how to enhance LLM capabilities through effective memory management.

## Prerequisites

- Python 3.10.12
- OpenAI API key (stored in `.env` file)
- Tavily API key (for web search functionality in Lab 5)

## Features

### 📚 Structured Learning Path

The course is organized into progressive labs:

- **Lab 1**: [Implementing self-editing memory from scratch](l1/L1.ipynb)
  - Breaking down the LLM context window
  - Adding memory to the context
  - Modifying memory with tools
  - Implementing an agentic loop

- **Lab 3**: [Building Agents with memory](l3/L3.ipynb)
  - Creating a simple agent with memory
  - Understanding agent state
  - Working with core memory
  - Working with archival memory

- **Lab 4**: [Programming Agent Memory](l4/L4.ipynb)
  - Understanding memory blocks
  - Working with ChatMemory
  - Defining custom memory modules
  - Creating agents with custom memory

- **Lab 5**: [Agentic RAG & External Memory](l5/L5.ipynb)
  - Loading data into archival memory
  - Connecting data via tools
  - Creating custom tools
  - Loading tools from Langchain
  - Creating research agents with web search capabilities

- **Lab 6**: [Multi-Agent Orchestration](l6/L6.ipynb)
  - Creating shared memory blocks between agents
  - Orchestrating multiple agents
  - Adding an orchestrator agent
  - Building a recruiting workflow with multiple specialized agents

## Setup Guide

1. Clone this repository:
   ```bash
   git clone https://github.com/corticalstack/llm-agent-memory-letta.git
   cd llm-agent-memory-letta
   ```

2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```
   
   Or using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file with your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

4. For Lab 5, you'll also need a Tavily API key:
   ```
   TAVILY_API_KEY=your_tavily_api_key_here
   ```

5. Launch Jupyter to run the notebooks:
   ```bash
   jupyter notebook
   ```

## Architecture

The repository is structured around the Letta framework, which provides tools for building LLM agents with different types of memory:

- **Core Memory**: Persistent information about the human and agent
- **Archival Memory**: Long-term storage for detailed information
- **Recall Memory**: Short-term memory for recent conversations
- **Custom Memory Blocks**: User-defined memory structures for specialized tasks

The labs progressively build on these concepts, introducing more complex memory systems and agent interactions.

## Resources

- [Letta Documentation](https://github.com/letta-ai/letta)