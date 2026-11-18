# Databricks pipeline incident response *(work in progress)*

An 11-job Databricks fleet (Bronze ingestion, Silver cleaning, a streaming job, Gold aggregates and a data-quality gate) processing eight monthly drops of about 127,000 rentals, with eight failures planted across code, data, streaming, duplicates and silent logic errors. This repo is the on-call record: how each failure showed up, what caused it, the change that fixed it, and the evidence that the fleet went from red to green.

> Scaffold only. It gets filled in as the fixes are made. Each incident gets a short postmortem in [docs/incidents/](docs/incidents/), using [the template](docs/incidents/TEMPLATE.md), and a row in [docs/fix_log.md](docs/fix_log.md).

## Planned layout

```
jobs/            my fixed job code and the exported job definitions (not the provided setup notebook)
docs/fix_log.md  one row per break: job, symptom, error class, root cause, change, evidence
docs/incidents/  one postmortem per break, with before and after snippets
docs/query_profile.md  rows read, join strategy, slowest step
docs/images/     red fleet, green fleet, query profile
```

## Credits

Built for ADSP 31011 Cloud-Native Data Engineering at the University of Chicago, Autumn 2026.
