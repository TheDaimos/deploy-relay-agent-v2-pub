# AGENTS.md — DRA V2 Public Release Repository

## Repository role

This repository is **release-only**. Public V2 development, issue triage, tests and development CI belong in `TheDaimos/deploy-relay-agent-v2-dev`. The existing `deploy-relay-agent-pub` remains the V1 HACS release repository.

This repository has been bootstrapped with **already-public V1.0.0 source**, not a published V2 release. Do not label, deploy, install, tag or announce it as V2 FINAL.

## Permanent release rules

1. Do not do feature development directly here. Promote only explicitly accepted, audited, exact public V2-DEV commits.
2. Maintain a record of source commit, changed files, byte or Git-blob parity and requested release version for every promotion.
3. Enforce accepted V2 security boundaries: LOCKED by default, explicit write approval, frozen source SHA, preview, backup before mutation, verify, rollback and RECOVERY_REQUIRED.
4. Never import private repository history, credentials, tokens, real diagnostics, backups, private extensions, user configuration or internal infrastructure.
5. Prior to release, validate Home Assistant/HACS compatibility, manifest and distribution metadata, license/branding, test outcomes and actual Home Assistant installation/migration/rollback.
6. No auto-release, auto-tag, auto-deploy or unattended Home Assistant restart. A release requires the user's explicit approval.
7. Use read-only GitHub Actions and standard public runners. Artifact upload only when the release process actually requires it; control storage and retention.
8. Keep V1 HACS distribution independent. Any V2 update path must preserve existing V1 project configuration and secure recovery.
9. `main` is not the `stable` tag, and a merged PR is not an authorization to issue a release.
10. Avoid calling the current V1-source baseline a V2 release. Do not create a public HACS integration package until all release gates pass.

Reference: `README.md`, `docs/PUBLIC_RELEASE_POLICY.md`, `docs/SOURCE_PROVENANCE.md`, `LICENSE`, `BRANDING.md`, `COPYRIGHT.md`.
