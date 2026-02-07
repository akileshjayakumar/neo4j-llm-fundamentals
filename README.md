# neo4j-llm-fundamentals
Hands-on Jupyter notebooks for learning how to build LLM workflows with Neo4j and LangChain.

## Quick Start
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env_neo4j .env
jupyter notebook
```

Open the `research/` folder in Jupyter and run notebooks in order.

## Core Capabilities
- Basic prompt and chain setup with LangChain + OpenAI (`01`, `02`).
- Retrieval-augmented generation using Neo4j vector search (`03`).
- Conversation memory and history storage in Neo4j (`04`, `05`).
- Tool-using agents and graph-backed agent flows (`06`, `07`).
- Cypher QA chain and prompt-instruction techniques (`08`, `09`, `10`).

## Configuration
Notebooks load variables from `.env`:

- `OPENAI_API_KEY` (required)
- `OPENAI_MODEL` (optional, default `gpt-4o`)
- `OPENAI_TEMPERATURE` (optional, default `0`)
- `NEO4J_URL` (required for graph/retrieval notebooks)
- `NEO4J_USERNAME` (required for graph/retrieval notebooks)
- `NEO4J_PASSWORD` (required for graph/retrieval notebooks)

`rag-text-files/` contains sample source text used by retriever notebooks.

## Usage Example
Recommended notebook progression:

1. `research/01_create_chain.ipynb`
2. `research/03_create_chain_with_retriever.ipynb`
3. `research/06_create_agent.ipynb`
4. `research/08_create_cypher_qa_chain.ipynb`

## Contributing and Testing
- Keep notebooks focused and incremental.
- Re-run notebook cells top-to-bottom before committing.
- If you add dependencies, update `requirements.txt`.

## License
This project is licensed under the MIT License. See `LICENSE` for details.
