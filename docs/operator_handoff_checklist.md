# Operator handoff checklist

## Project

- Title: Hospital Intake Agent Runtime
- Domain: Healthcare Operations AI

## Why this exists

Serve structured intake assistants that triage symptoms, collect missing context, and route patients to the right next step.

## Handoff checklist

1. Confirm the top model or retrieval output is grounded in the right business context.
2. Record the main decision the operator should make next.
3. Capture any escalation trigger that requires a human specialist.
4. Note the business metric that would be harmed if this decision is wrong.
5. Save a short summary that another operator can continue without re-running the full analysis.

## Expected output

- top finding
- next action
- escalation trigger
- owner
- business impact note
