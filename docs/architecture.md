# Architecture

## Problem framing

- User: Hospital intake coordinators and digital access teams
- Problem: Hospitals need symptom intake agents that stay structured, safe, and fast during patient routing.
- Decision: Route each patient to self-care, urgent clinic, or ED escalation based on the intake flow.

## System flow

1. A user submits case context, business signals, or a search question.
2. The API exposes scoring, analysis, and recommendation endpoints.
3. The web application turns those outputs into an operator-facing workflow.
4. Observability, docs, and runbooks make the project easier to evaluate and extend.

## Production posture

- Separate app, docs, demo, and data folders
- Container-ready packaging
- API endpoints for health and workflow actions
- Screenshot-ready demo surface
- Research and upstream audit artifacts included in-repo
