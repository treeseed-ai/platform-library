---
schemaVersion: treeseed.knowledge-page/v1
id: admin-migration-development-release-generation-81
bookId: platform-integration
slug: admin-migration-development-release-generation-81
title: "Historical: Admin migration and development/release generation 81"
summary: Historical generation-81 acceptance record, preserved for provenance;
  superseded by later Platform compositions.
status: published
visibility: team
order: 10
contributors:
  - adrian-webb
  - codex
relatedBookIds: []
relatedKnowledgeIds: []
relatedNoteIds: []
relatedQuestionIds: []
relatedObjectiveIds: []
relatedProposalIds: []
relatedDecisionIds: []
guaranteeIds:
  - guarantee.user.auth.register-user.001
  - guarantee.user.auth.verify-email.002
  - guarantee.user.auth.forgot-reset-password.003
  - guarantee.user.auth.user-login.004
  - guarantee.user.auth.user-logout.005
  - guarantee.team.team.team-management-production-readiness.022
audiences:
  primary:
    - developers
    - operators
    - agents
  secondary:
    - reviewers
  excluded: []
capabilityIds:
  - authentication
  - accounts
  - teams
  - agent-monitoring
  - development-runtime
  - release-custody
routePatterns:
  - /auth/**
  - /app/account/**
  - /app/teams/**
  - /app/work/**
resourceTypes:
  - platform-generation
  - guarantee-run
  - communication-send
  - agent-invocation
  - capacity-assignment
actionIds:
  - monitor
  - review
  - reconcile
  - rollback
keywords:
  - generation 81
  - admin migration
  - reviewer
  - agent communication
  - platform manager
documentationUrls: []
---

Historical checkpoint recovered from archived commit e6c5d6a4d504805108d602f80599c8faa56c4420. The following records generation 81 only; it is not current setup guidance or a claim that these historical gates were rerun. Host-specific paths and runtime identifiers below are historical evidence, not installation defaults.

## Exact composition

Platform staging merge `43691da87ad5c145b3511311f4f28489564bf23a` contains candidate `ccbe3c009f8914b4b1ae8440da22e6e211126f16`. The development integration release is generation 81 and binds Deployment staging merge `e3fdb7ba1abe87783ec46bd38ff3f26a254a382e` / `0.1.0-rc.111`.

The exact host payloads are SDK `0.13.0-rc.51`, UI `0.12.18-rc.9`, Core `0.12.60-rc.6`, Admin `0.12.59-rc.20`, API `0.8.0-rc.49`, CLI `0.13.0-rc.29`, Agent `0.13.0-rc.25`, TreeDX `0.3.0-rc.11`, Reviewer `0.1.0-rc.13`, and TreeAI `0.1.0-rc.4`. The active known-good receipt is `receipt-1787892345015`; catalog digest `sha256:e01c8ff6ca68284efcf889d4becc5e1d08cdf28d9f28db98fa85addc897f3f00`; configuration digest `sha256:899c32d0b026de708982760e61ac9619c3d3b284ba73e6a9c435cc951214e11d`.

## Acceptance evidence

Immutable runs `gen81-desktop-chromium-20260828-r3`, `gen81-tablet-chromium-20260828`, and `gen81-mobile-chromium-20260828` each passed 22 of 22 active authentication, account, and team guarantees. The aggregate is 66 passed, zero failed, and zero blocked. Planned/future guarantees remain planned.

Reviewer workplan `2026-08-28T05-20-33-758Z-generation-81-authenticated-platform-baseline` was generated from the desktop run. Its evidence manifest contains two copied objects with SHA-256 custody. Reviewer remains loopback-only; Admin exposes its handoff only when a loopback Reviewer URL is configured.

## Communication monitoring foundation

Catalog reads proved SDK send `send-1801e17f633fdec25a232b77843a3ba0`, invocation `invocation-e991785bcad120935e791f4c46034d37`, agent `technical-writer`, and assignment `assignment_WXj8uUgIIazqzLcYVksuGcMoz2AB-PT7`. The send is complete with one response, the invocation outcome is responded, the agent definition revision is `11a98caca3d0b5a46934078a2a41e966d2098db6`, and provider `codex-local` is communication-ready.

The assignment is returned with a released lease. Its synthetic communication workday has one exact usage record and one `task_completed_actual_settlement` ledger entry, both recording six active and elapsed seconds. The TreeDX workspace and capability handles are revoked. No assignment, lease, workspace, or capability residue remains. No catalogued team workday existed, so Admin must display that field as unavailable rather than inventing a zero value.

## Operator and agent context

Use the manager-owned `/usr/bin/trsd` wrapper so the canonical API URL and localhost CA are applied. On this workstation `~/.local/bin/trsd` points to that wrapper because a stale npm-global CLI previously shadowed it and produced `fetch failed` against `127.0.0.1:3002`.

The authoritative Platform library binding is repository `repo_c3626e5d3fa0dc9e`, tracking `refs/remotes/origin/staging`. At certification it resolved `b4e32c8b8d3031fc142230595b2fc34f5f728c9b` with a ready, non-stale search index. Always verify `trsd library status platform` and use the returned exact commit for reproducible reads.

Generation 73 remains available as an exact Git/catalog rollback lock at Platform commit `0af2640405503e72a13b455193355f944bd41a94`, and historical receipt `receipt-1787861393566.json` remains retained. Its live rollback and final restoration were proven during Deployment rc110/rc111 acceptance. Generation 81 is the new certified integration point for authenticated agent chat work.

