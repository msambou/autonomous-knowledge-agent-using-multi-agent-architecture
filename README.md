# Autonomous Knowledge Agent Using Agentic AI Pattern

## Project Introduction
In this project, I'll develop UDA-Hub, an intelligent, multi-agent decision suite capable of resolving customer support tickets across multiple platforms.

**Key Capabilities:**

1. Multi-Agent Architecture with LangGraph Design and orchestrate specialized agents (e.g., Supervisor, Classifier, Resolver, Escalation…).

2. Input Handling Accept incoming support tickets in natural language with metadata (e.g., platform, urgency, history).

3. Decision Routing and Resolution

    * Route tickets to the right agent based on classification
    * Retrieve relevant knowledge via RAG if needed
    * Resolve or escalate based on confidence and context
    * Memory Integration

4. Maintain state during steps of the execution
    * Short-term memory is used as context to keep conversation running during the same session
    * Store and recall long-term memory for preferences, as an example