---
schemaVersion: treeseed.knowledge-page/v1
id: repository-checkpoint-reconciliation
bookId: platform-delivery-history
slug: repository-checkpoint-reconciliation
title: Repository checkpoint reconciliation
summary: How archived library checkpoints were preserved and reconciled without
  restoring retired execution schemas or backup branches.
status: published
visibility: team
order: 100
contributors: []
relatedBookIds: []
relatedKnowledgeIds: []
relatedNoteIds: []
relatedQuestionIds: []
relatedObjectiveIds: []
relatedProposalIds: []
relatedDecisionIds: []
guaranteeIds: []
audiences:
  primary: []
  secondary: []
  excluded: []
capabilityIds: []
routePatterns: []
resourceTypes: []
actionIds: []
keywords: []
documentationUrls: []
---

## Preservation and reconciliation

The organization cleanup retained complete, independently restore-tested Git bundles before deleting obsolete library refs. Thirteen library archives contained no missing substantive blobs; their only unique file was an initialization marker. Team Library revision 1 was superseded by revision 2. SDK context-query, query-set and test differences were trailing whitespace; retired execution.requiredCapabilities fields and removed workspace-tool grants were not restored.

The missing SDK Core book and objective were restored through TreeDX publication at `a2769cba7a6a70e56317aaec6aa1b3a259a91f77`. Platform generation-81 evidence was restored with historical-only framing at `34432111e97e8c2430e164434d1dbf2c9ca76ed3`. The eight Platform delivery-history records were restored at `2ff565817a53b8d26554d74fdc66a4db5bc58b25`, preserving all seven Markdown bodies and current staging ancestry.

Historical discussion events remain recoverable from the archived bundles; they must not be replayed as new messages or assignments. Retired Market draft guarantees remain historical evidence, not current CLI, licensing or hosted-routing policy.

## Publication ownership

API [#273](https://github.com/treeseed-ai/api/pull/273) removed per-commit GitHub backup-branch replication. GitHub publication follows the configured protected integration branch with exact-head checks. R2 replication remains separate; an unpublished draft is not falsely described as an off-host backup.

API [#276](https://github.com/treeseed-ai/api/pull/276) removed remaining human/editorial staging admission gates. Authorization, immutable revision checks, workspace concurrency, expected remote heads, storage and index validation remain enforced. Human review belongs only to production/main promotion.

## Delivery evidence

API rc95 was promoted from `4a24282050675e2b64b733d4d6d6fd36f1988e9f` without rebuilding accepted OCI artifacts. [Platform #463](https://github.com/treeseed-ai/platform/pull/463) and [#464](https://github.com/treeseed-ai/platform/pull/464) bind generation 226 and Deployment rc275. [Platform #462](https://github.com/treeseed-ai/platform/issues/462) is the authoritative work and acceptance record. Retain recovery bundles; publication of recovered content is not authorization to delete the only remaining historical copy.

