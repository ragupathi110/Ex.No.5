# EXP 5: COMPARATIVE ANALYSIS OF DIFFERENT TYPES OF PROMPTING PATTERNS AND EXPLAIN WITH VARIOUS TEST SCENARIOS

# DATE : 05/05/2025

# REGISTER NUMBER : 212222060185

### Introduction:

Prompting refers to the method used to communicate tasks to large language models (LLMs) like ChatGPT. Different prompting techniques can dramatically impact the model's performance and accuracy. This document provides a comparative analysis of various prompting patterns, their advantages, limitations, and effectiveness across diverse test scenarios.

### Types of Prompting Patterns

### Zero-shot Prompting

•	Definition: No example is provided. The task is described directly.

•	Use Case: Simple queries where the task is obvious.

•	Example: "Translate this sentence to Spanish: 'Good morning.'"

•	Strengths: Fast, no need for training data.

•	Weaknesses: Prone to misunderstanding in complex tasks.

### One-shot Prompting

•	Definition: A single example is included before the prompt.

•	Use Case: Slightly complex tasks requiring hinting.

•	Example: "Translate: 'Hello' → 'Hola'. Now translate: 'Goodbye' →"

### Few-shot Prompting

•	Definition: Multiple examples are provided.

•	Use Case: Pattern recognition tasks like classification.

•	Example: Several sentiment-labeled sentences followed by a new sentence.

### Chain-of-Thought (CoT) Prompting

•	Definition: Encourages the model to show intermediate reasoning steps.

•	Use Case: Math, logic, multi-step reasoning.

•	Example: "Tom has 5 apples and gives away 2..."

### Self-Consistency

•	Definition: Run CoT multiple times and aggregate results.

•	Use Case: Increases reliability for reasoning tasks.

### ReAct (Reason + Act)

•	Definition: Combines reasoning with actions like using tools.

•	Use Case: Real-time tasks needing external data.

### Instruction Prompting

•	Definition: Task is given as a clear instruction.

•	Use Case: Document summarization, rewriting, etc.

•	Example: "Summarize this article in 3 bullet points."

### Retrieval-Augmented Generation (RAG)

•	Definition: Model retrieves relevant documents before answering.

•	Use Case: Requires up-to-date information.

•	Example: "Who won the latest Super Bowl?"

### Test Scenarios and Pattern Comparison

Text Classification Task (Sentiment Analysis)

•	Input: "I love this product!"

•	Zero-shot: May return 'Positive'.

•	Few-shot: More accurate by showing similar examples.

•	CoT: Analyzes words like 'love'.

•	Self-Consistency: Confirms 'Positive' across responses

### Math Reasoning

•	Input: "What is 24 divided by 6 plus 3?"

•	Zero-shot: Might return wrong order (e.g., 24 / (6+3)).

•	CoT: Explains: 24 ÷ 6 = 4, 4 + 3 = 7.

•	Self-Consistency: Aggregates multiple CoTs to ensure correct answer.

### Planning a Trip

•	Input: "Plan a weekend trip to NYC under $500."

•	Zero-shot: Basic itinerary.

•	Instruction Prompting: More structured plan.

•	AutoGPT-style: Breaks down tasks, checks prices, suggests.

•	RAG: Retrieves live hotel/transport data.

### Real-Time Information

•	Input: "What is the current price of Bitcoin?"

•	Zero-shot: Likely outdated.

•	ReAct: Uses search API.

•	RAG: Fetches real-time info from verified sources.

### Historical Analysis

•	Input: "Causes of World War I."

•	Few-shot: Offers detailed breakdown with examples.

•	CoT: Reasoned explanation: nationalism, alliances, etc.

•	RAG: References external historical texts.

### Comparative Summary

![image](https://github.com/user-attachments/assets/dba95092-2ed5-4e21-a62e-dc923ba2cd59)




### Advanced Prompt Engineering Techniques

•	Prompt tuning and prefix tuning

•	Embedding instructions in tokens

•	Contrastive prompt learning

•	Prompt chaining for modular workflows

### Prompt Evaluation Metrics

•	Accuracy

•	Relevance

•	Faithfulness (non-hallucination)

•	Consistency across runs

•	Latency and token cost

### Prompting Challenges and Limitations

•	Sensitivity to phrasing

•	Context window limitations

•	Bias and fairness

•	Prompt hacking or prompt injection vulnerabilities

###  Prompting for Specific Domains

•	Healthcare: Medical question answering, diagnosis support

•	Legal: Summarizing legal documents, interpreting clauses

•	Education: Tutoring, exam generation

•	Creative Writing: Story expansion, poem composition

### Tool-Augmented Prompting (LLM Agents)

•	LangChain, AutoGPT, AgentGPT

•	Memory-augmented prompting

•	API orchestration using prompts

### Future Trends in Prompting

•	Multi-modal prompting (text, image, audio)

•	Reinforcement learning from human feedback (RLHF)

•	Prompt marketplaces and reusable templates
 

### Conclusion

Each prompting pattern serves a unique purpose. Zero-shot and instruction prompts are ideal for general use, while CoT and self-consistency improve reasoning tasks. Few-shot enhances performance where examples exist, and ReAct/RAG patterns support real-time, interactive applications. Understanding the right pattern for a task is essential for maximizing the effectiveness of LLMs.

 References
•	OpenAI Technical Reports
•	Google Research on Chain-of-Thought Prompting
•	Stanford NLP Group Papers
•	ReAct: Reasoning and Acting with Language Models (Yao et al.)
•	AutoGPT Open Source Documentation
