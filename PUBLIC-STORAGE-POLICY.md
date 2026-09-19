# PDF Storage Policy — Public Distribution Only

This repository is the **public PDF distribution pool** for Rechercher.

## Allowed

Only PDFs whose acquisition manifest explicitly records:

- `public_download: true`
- `storage_visibility: publication-eligible`
- rights status permitting redistribution
- real PDF signature and successful PDF validation

## Forbidden

The following must never be persisted here:

- `research-only` material
- `rights-unclear` material
- `rights-review-required` material
- encrypted research vault files (`.pdf.enc`, `.enc`, `.encrypted`)
- unverified or invalid PDFs

Those records belong in the separate private **Developer Review Vault**.

This repository must never be used as a fallback for protected material.
