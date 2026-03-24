# Automated Expense Categorizer

## Solution Summary
Production-ready domain application.

This Phase-2 implementation is a domain-ready, deployable web application for **AI & Data** workflows.

## Core Capabilities
- Responsive dashboard with KPI cards and recent activity table
- Domain record lifecycle with full CRUD (web + API)
- Dynamic schema fields tailored to this use case
- Status pipeline: `new, processing, validated, deployed`
- Docker + Gunicorn deployment assets, CI checks, and Pytest tests

## Domain Model
- Primary entity: **Automated Expense Insight**
- Collection: **Automated Expense Insights**
- Dynamic fields:
- Source Input (`source_input` / textarea)
- Model Output (`model_output` / textarea)
- Confidence Score (`confidence_score` / number)

## Operational Workflow
1. Capture source data
2. Run analysis
3. Review confidence
4. Publish insight

## API
- `GET /api/health`
- `GET /api/schema`
- `GET /api/records`
- `POST /api/records`
- `GET /api/metrics`

## Run Locally
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

## Docker Run
```bash
docker compose up --build
```

## Proof of Concept
- [proof-of-concept.md](proof-of-concept.md)
- [proof/demo-output.txt](proof/demo-output.txt)
- [proof/ui-preview.svg](proof/ui-preview.svg)
