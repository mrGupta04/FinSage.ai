# FinSage.ai - Multi-Agent MVP Scaffold

This repository contains a small Python scaffold implementing the core of the FinSage multi-agent architecture for experimentation and incremental development.

What's included (MVP):

- Planner (orchestrator) — decomposes queries and coordinates agents
- DataAgent — mock structured financial data retrieval
- DocumentAgent — mock unstructured document extraction (RAG placeholder)
- CalculationAgent — financial computations (ratios, DCF stub)
- ReasoningAgent — simple logical synthesis
- CLI — run a sample query
- Minimal unit test for CalculationAgent

This scaffold uses pure Python and minimal dependencies so you can run it locally and extend each agent with real connectors (Yahoo Finance, SEC Edgar, vector DBs, ML models) later.

How to run

Open PowerShell in the project root and run:

```powershell
python cli.py
```

Run tests (if you have pytest installed):

```powershell
python -m pytest -q
```

Next steps

- Replace mock implementations with real API clients
- Add DocumentAgent RAG stack (embeddings + vector DB)
- Add PredictionAgent and NewsAgent
- Add ValidationAgent and risk/comparison agents

License: MIT (adapt as needed)
