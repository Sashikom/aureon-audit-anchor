# AUREON Audit Anchor Repository

This repository stores public, content-minimized AUREON audit-anchor records. An anchor contains a SHA-256 digest and limited metadata; it must not contain trading payloads, credentials, API tokens, or private keys.

## First anchor record

- Record: `aureon-anchors/aureon-phase4-export/anchor.json`
- Hash algorithm: SHA-256
- Anchored journal entries: 1
- The record refers to a locally verified Phase 4 audit export from AUREON checkpoint 87. It is a bootstrap anchor; publication in this repository becomes external only after a GitHub commit is actually created and its commit SHA is independently retained and verified.

## Verification notes

The anchor record's own `anchor_hash` protects the canonical metadata representation. It does not make GitHub history immutable: repository administrators can change or delete content. Preserve the commit SHA independently. This repository is not a proof of profitability, trading correctness, legal validity, or zero-loss operation.

## Publishing

Upload these files to the empty repository `Sashikom/aureon-audit-anchor` and commit them. Then record the resulting commit SHA and verify the committed `anchor.json` by downloading it from the public repository. Do not upload credentials or full recovery/trading payloads.
