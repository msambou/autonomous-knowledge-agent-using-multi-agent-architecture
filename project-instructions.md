Project Instructions
Your starter folder looks like the following structure:

starter/
├── agentic/
│   ├── agents/
│   ├── design/
│   ├── tools/
│   └── workflow.py
├── data/
│   ├── core/
│   ├── external/
│   └── models/
├── .env
├── 01_external_db_setup.ipynb
├── 02_core_db_setup.ipynb
├── 03_agentic_app.ipynb
└── utils.py

Design
Start by designing the solution. Your implementation will follow it.
Place all the documentation and diagrams about the design of your agentic system inside agentic/design
Setup
Run notebook 01_external_db_setup.ipynb in order to have all the data related to the account Cultpass. It's the first customer that has purchased Uda-hub
Run notebook 02_core_db_setup.ipynb in order to have all the data related to Uda-hub application, including the files "received" from Cultpass like cultpass_articles.jsonl
You need to expand cultpass_articles form 4 to at least 14 articles. Make sure you have diverse topics for your agentic system.
Agentic Workflow
Develop your agents inside agentic/agents and your tools inside agentic/tools . This will help you with modularity.
Develop your workflow orchestration in the file workflow.py . There's already a sample for you, but donot use it, create the graph from scratch. Do not use the prebuilt workflow.
When developing tools that abstract the database both for retrieval or for actions, please mind the relative/absolute paths. I strongly recommend you to use something like MCP servers for the tools.
If you're using RAG for retrieval, make sure you have documented how it works.
For short-term memory (session), you can use thread_id. For long-term memory, you're free to use semantic search.
Run
There's a chat_interface() function inside utils.py. It's just a simple while True block. Starter code imports this inside the notebook. Feel free to improve it!
You're not forced to use 03_agentic_app.ipynb , you can develop inside a .py module, but please name it as 03_agentic_app.py and make it explicit how to run your project.
You must create test cases to pass the project!