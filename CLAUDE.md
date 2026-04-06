# Repository Governance Guidance

## Canonical Governance Inputs

- Treat `.devops/index/file-index.json` as the canonical file graph snapshot.
- Treat `.devops/policies/ownership-map.yaml`, `.devops/policies/gate-rules.yaml`, and `.devops/graph/manifests/capability-map.yaml` as canonical governance data.
- Treat `AGENTS.md`, `CLAUDE.md`, and `.github/*` as generated projections. Regenerate them instead of editing by hand.

## Execution Rules

1. Configure provider credentials before analysis.
2. Use linked git worktrees for any write-capable repo flow.
3. Preview and verify generated projections before publish.
4. When present, consult `.devops/suites/*/PLAYBOOK.md` before changing governed behavior.

## Capability Owners

- owner-backend-api: backend.api -> 1 files | github @nyartsgnaw
- owner-domain-logic: domain.logic -> 1 files | github @nyartsgnaw
- owner-external-integration: external.integration -> 1 files | github @nyartsgnaw
- owner-infra-workflow: infra.workflow -> 1 files | github @nyartsgnaw
- owner-llm-modeling: llm.modeling -> 1 files | github @nyartsgnaw

## Required Checks

- check-backend-api
- check-domain-logic
- check-external-integration
- check-infra-workflow
- check-llm-modeling
