# Runbook

## Target user

Hospital intake coordinators and digital access teams

## Core operating loop

1. Load or bootstrap sample data.
2. Start the FastAPI application.
3. Use the web interface to score, analyze, and draft the next action.
4. Review health status before demo or deployment.

## Operator note

The main value of this repo is the workflow it supports: Route each patient to self-care, urgent clinic, or ED escalation based on the intake flow.. Keep the UI, docs, and API aligned with that business action.
