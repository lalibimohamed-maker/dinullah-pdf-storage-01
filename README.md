# dinullah-pdf-storage-01

Dedicated storage for the books acquired by Rechercher for موسوعة دينُ الله, from the Prophetic era through the present.

## Storage routes

This storage has two logical access routes:

- **Public route**: for PDFs whose verified rights permit public redistribution.
- **Protected route**: for PDFs that must remain developer/private. The protected route MUST use a permissioned/private backend; this public GitHub repository is never used as the protected backend.

The two routes are **access states, not two PDF copies**.

## Repository-owned Releases

This storage repository retains its own GitHub Releases. Releases are a persistent distribution/storage mechanism for verified assets and are not removed or replaced by Releases in another storage shard. The repository's storage-release-publisher.yml workflow publishes eligible assets as Release assets.

## One-PDF-only rule

- Exactly one canonical plaintext `.pdf` is retained per SHA-256.
- Public and protected routes MUST NOT contain duplicate physical copies of the same SHA-256.
- `.pdf.enc` is forbidden.
- If rights change, the access state may change without creating a second PDF.
- SHA-256, provenance, rights, validation, and acquisition metadata remain the source of truth.
- Rights-unclear or non-redistributable material must never be published on the public route.

## Developer access

The developer has repository administration/read/write access to this repository. Protected access is permitted only through the separate permissioned backend and must be granted to the same developer identity.

## Corpus boundary

This repository never writes directly to the main Corpus.
