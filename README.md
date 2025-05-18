# ContentCreationAgent
Fully local Youtube and Instagram Content Creation using Reflexion Agent

## Summary
This file orchestrates an AI-driven, reflexive content creation pipeline, from answering a query to producing platform-optimized, viral content for YouTube and Instagram—all running locally, without relying on external cloud-based LLMs.

## Contents
The file, ContentCreation.ipynb, implements a "Content Creator With Reflexion"—a workflow to generate detailed, high-quality content for YouTube and Instagram using AI agents and tools, with a focus on self-critique and iterative improvement.

Here’s a summary of what the notebook does:

### Data Models with Pydantic:
It defines schemas (AnswerQuestion, ReviseAnswer) that structure how answers are generated, critiqued, and revised.

### Prompt Chains and Templates:
The notebook sets up prompt templates using LangChain for generating detailed answers, critiquing those answers, and revising them to include improvements and references.

### AI Model Integration:
It uses locally hosted large language models (LLMs) like "qwen3:14b" and "llama3.2:3b-instruct-fp16" for both content generation and output formatting.

### Tool Integration:
The notebook integrates with search APIs (e.g., Tavily) to fetch external information based on the model’s search queries.

### Graph Workflow:
It builds a multi-step workflow/graph:

1. Draft an answer.
2. Use tools to enhance the answer with additional info.
3. Revise the answer based on critiques.
4. Generate final viral content suitable for social media.

Testing and Output:
The notebook includes example runs, showing how the system answers queries like "Maintaining a healthy lifestyle in Bangalore for corporate professionals" and turns them into fully structured, ready-to-publish scripts and captions.
