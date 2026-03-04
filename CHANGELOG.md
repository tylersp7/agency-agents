# Changelog

## 2026-03-04 — Security Hardening

### Added
- `security/SECURITY-BASELINE.md` — Shared security rules for all agents covering prompt injection resistance, human approval gates, data handling, scope boundaries, and agent handoff integrity
- Security sections added to all 55+ agent files across 3 risk tiers
- 4 human approval gates (`# HUMAN GATE`) in agents-orchestrator.md at every phase boundary
- Security & Trust Protocol subsection in agents-orchestrator.md
- Security Gate subsection in strategy/nexus-strategy.md quality gates
- Security Verification checklist in strategy/coordination/handoff-templates.md
- Operational note in specialized/agentic-identity-trust.md connecting it to orchestrator and security baseline
- `docs/plans/2026-03-04-security-hardening-design.md` — Design document
- `docs/plans/2026-03-04-security-hardening-plan.md` — Implementation plan
- Security section in README.md

### Changed
- `engineering/engineering-devops-automator.md` — Terraform ALB example now uses `enable_deletion_protection = true` (was `false`)
- `support/support-legal-compliance-checker.md` — Placeholder credentials (`dpo@company.com`, `1-800-PRIVACY`) replaced with explicit `[REPLACE]` markers

### Security Tiers
- **Tier 1 (7 agents)**: Deep agent-specific security constraints for orchestrator, devops-automator, sales-data-extraction, report-distribution, data-consolidation, ai-engineer, backend-architect
- **Tier 2 (14 agents)**: Targeted security rules for senior-developer, frontend-developer, mobile-app-builder, rapid-prototyper, finance-tracker, legal-compliance-checker, and all 8 marketing agents
- **Tier 3 (~34 agents)**: Security baseline reference added to all remaining agents
