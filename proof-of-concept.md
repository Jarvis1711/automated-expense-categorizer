# Proof of Concept - Automated Expense Categorizer

## Scope
- App category: AI & Data
- Entity model: Automated Expense Insight
- Deployable stack: Flask + SQLAlchemy + Gunicorn + Docker + CI

## Dynamic Field Configuration
- Source Input: `source_input` (textarea)
- Model Output: `model_output` (textarea)
- Confidence Score: `confidence_score` (number)

## Run Evidence Commands
```bash
python app.py
curl http://localhost:5000/api/health
curl http://localhost:5000/api/schema
curl -X POST http://localhost:5000/api/records   -H "Content-Type: application/json"   -d '{"title":"Demo Record","status":"processing","payload":{"source_input":"Demo value","model_output":12,"confidence_score":"seed note"}}'
curl http://localhost:5000/api/metrics
```

## Metadata
- Idea number: 10
- Generated UTC: 2026-03-24T15:52:21.794798+00:00
- Status: Phase-2 complete
