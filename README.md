# Hospital Intake Agent Runtime

![Demo Screenshot](demo/screenshot.png)

## Overview

Serve structured intake assistants that triage symptoms, collect missing context, and route patients to the right next step.

## Real-world problem

- User: Hospital intake coordinators and digital access teams
- Problem: Hospitals need symptom intake agents that stay structured, safe, and fast during patient routing.
- Decision improved: Route each patient to self-care, urgent clinic, or ED escalation based on the intake flow.
- KPI target: Reduce intake delays and improve routing accuracy.

## Why this matters

This repo is positioned as a real product for a real team, not a framework-only demo. The goal is to show how research-backed AI, analytics, or graph systems become deployable workflows with docs, UI, screenshots, and business-facing outputs.

## Project profile

- Domain: Healthcare Operations AI
- Project type: `llm`
- Tags: healthcare, triage, agents, serving

## Workflow

1. Ingest the operational context for the user and case.
2. Score risk, quality, or opportunity using the project API.
3. Compare current signals against a business baseline.
4. Generate a recommendation or operator brief for the next step.

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python scripts/bootstrap_data.py
uvicorn src.app.main:app --host 0.0.0.0 --port 8000 --reload
```

Open `http://localhost:8000/` to use the interactive application.

## Key endpoints

- `GET /`
- `GET /health`
- `GET /bootstrap`
- `GET /project`
- `POST /score`
- `POST /analyze`
- `POST /query`
- `POST /recommend`

## Documentation

- [Architecture](docs/architecture.md)
- [Evaluation](docs/evaluation.md)
- [Runbook](docs/runbook.md)
- [Innovation memo](research/innovation_memo.md)
- [Upstream audit](research/upstream_audit.md)
