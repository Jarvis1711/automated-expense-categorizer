# Proof of Concept - Automated Expense Categorizer

## Deployment Readiness
- Web app + API routes active
- Container and PaaS deployment files included
- Automated test suite and CI workflow included

## Smoke Commands
```bash
python run.py
curl http://localhost:5000/api/health
curl http://localhost:5000/api/schema
curl -X POST http://localhost:5000/api/items   -H "Content-Type: application/json"   -d '{"title":"Phase3 Demo","status":"new","payload":{"owner":"sample","impact_score":5,"notes":"notes"}}'
curl http://localhost:5000/api/metrics
```

## Metadata
- Generated UTC: 2026-03-24T16:15:10.966664+00:00
- Phase: 3
- Domain: General
