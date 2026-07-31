# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **Support / On-call Engineer** triggers incident response and notifies the **Release Manager / Release Coordinator**
  - Rollback to last known-good release if necessary (executed by the **Support / On-call Engineer** per the rollback plan owned by the **Release Manager**)
  - Triage root cause and capture action items

See [OctoAcme Personas](octoacme-roles-and-personas.md) for the responsibilities of the [Support / On-call Engineer](octoacme-roles-and-personas.md#support--on-call-engineer) and [Release Manager / Release Coordinator](octoacme-roles-and-personas.md#release-manager--release-coordinator).

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
