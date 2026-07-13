# Release & Deployment Checklist (proposed)

Purpose: a concise, repeatable checklist to reduce release risk and ensure cross-functional readiness.

Pre-release
- [ ] Link PRs and issues that are part of this release.
- [ ] Release Engineer has validated build artifacts and tagging.
- [ ] All linked PRs have CI green and required approvals.
- [ ] Security scans completed and any findings triaged.
- [ ] Accessibility quick-check completed for user-facing changes.
- [ ] Observability: required metrics/instrumentation implemented and dashboards created.
- [ ] QA smoke tests defined and scheduled for staging.

Deployment
- [ ] Deployment window scheduled and communicated to stakeholders.
- [ ] Backups/snapshots taken if applicable.
- [ ] Release Engineer or on-call runs pre-deploy checklist.
- [ ] Deploy to staging and run smoke tests (QA sign-off).
- [ ] Deploy to production (automated pipeline preferred).

Post-deploy
- [ ] Run post-deploy verification (smoke checks and critical SLOs).
- [ ] Monitor dashboards and alerts for 30–60 minutes.
- [ ] Announce release to stakeholders and support channels.
- [ ] Update release notes and link to runbooks/runbooks updated if relevant.

Rollback / Incident
- [ ] Rollback plan reviewed and verified.
- [ ] Incident contacts and on-call rotation notified if anomalies detected.
- [ ] Capture post-release action items and assign owners.

Recommended owners:
- Release Engineer: overall owner of checklist execution.
- Project Manager: owner of communication and stakeholder updates.
- QA: owner of smoke tests and verification.
- Observability Engineer: owner of dashboards and alerting verification.
