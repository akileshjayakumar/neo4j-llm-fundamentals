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

## Capabilities
- Basic prompt and chain setup with LangChain + OpenAI (`01`, `02`).
- Retrieval-augmented generation using Neo4j vector search (`03`).
- Conversation memory and history storage in Neo4j (`04`, `05`).
- Tool-using agents and graph-backed agent flows (`06`, `07`).

## Configuration
- `OPENAI_API_KEY`: Required for related integrations/features.
- `OPENAI_MODEL`: Required for related integrations/features.
- `OPENAI_TEMPERATURE`: Required for related integrations/features.

## Usage
```bash
python -m pytest
```

## Contributing and Testing
- Contributions are welcome through pull requests with clear, scoped changes.
- Run the following checks before submitting changes:
```bash
python -m pytest
```

## License
Licensed under the `MIT` license. See [LICENSE](./LICENSE) for full text.
