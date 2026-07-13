# Observability & Monitoring Checklist (proposed)

Purpose: ensure features ship with the telemetry and runbook items required for operability.

Instrumentation
- [ ] Identify key business and technical metrics (SLOs/SLIs).
- [ ] Define events and logs to capture critical user flows.
- [ ] Implement traces for long-running requests or important flows.
- [ ] Add label/metadata to logs for easier filtering (request id, user id where allowed).

Dashboards & Alerts
- [ ] Create dashboard(s) for the feature's health and usage.
- [ ] Define alert thresholds and test alert triggers.
- [ ] Link alerts to runbooks with triage steps and escalation contacts.

Runbooks & On-call
- [ ] Create or update runbook with reproduction steps and mitigation guidance.
- [ ] Ensure on-call knows who to escalate to (observability, release, security).
- [ ] Post-release: review alert noise and tune thresholds.

Ownership
- Observability Engineer: telemetry design and alert tuning.
- Developers: implement instrumentation.
- Data Analyst: validate metric definitions/dashboards.
