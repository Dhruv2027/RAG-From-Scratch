# RAG-from-Scratch: Building a Custom Retrieval Augmented Generation Pipeline
This repository contains a Jupyter notebook where I attempt to create a Retrieval Augmented Generation (RAG) pipeline from the ground up, without relying on pre-built text-splitting and chunking features from tools like LangChain. The goal of this project was to gain a deeper understanding of the mechanics behind RAG pipelines, rather than creating a polished, production-ready system.

## Project Overview

In this project, I used a PDF file for Harry Potter and the Sorcerer's Stone as my dataset to build the RAG pipeline. The focus was on understanding how large language models (LLMs) manage token context length, and how to optimize the prompts and context size for each specific LLM to maximize performance.

Some of the key learnings included:

How tokenization works with LLMs
- The balance between prompt length and context size
- Techniques to enhance retrieval accuracy by refining prompt construction

I asked the system several nuanced questions, such as:
- "Which vault was the Sorcerer's Stone kept in at Gringotts Bank?"
- "When was Harry's first Quidditch match?"
Despite the simplicity of the setup, the system successfully returned accurate responses, demonstrating the core principles of RAG in action.

## How to Run the Notebook
Clone this repository to your local machine:
```
git clone [<repository-url>](https://github.com/Dhruv2027/RAG-From-Scratch.git)
```

Install the required Python dependencies:
```
pip install -r requirements.txt
```
Download and set up the Ollama platform, which is used for running the LLM models. You will need to:
Download the Ollama platform [here](https://ollama.com/)
Run the following commands in your terminal:
```
ollama run mistral
ollama pull nomic-embed-text
```

Open the Jupyter notebook and run each cell to follow along with the code. The notebook is designed with clear, beginner-friendly documentation to guide you through the process.

## Notes for Users
This project was designed for educational purposes to explore the fundamental concepts behind a RAG pipeline. While the current implementation works well for basic tasks, it may require further refinement for real-world applications.

Feel free to explore the code, experiment with different datasets, and enhance the pipeline to suit your needs!
