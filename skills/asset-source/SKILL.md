---
name: asset-source
description: Record and review source, license, hashes, derivatives, and publication boundaries for Toymoil media assets.
---

# Asset Source

Read docs/08_ASSET_POLICY.md before acquiring or generating an asset.

## Required record

Capture source URL or generator, author/provider, acquisition date, exact license,
license text location, original SHA-256, selected-file SHA-256, derivative steps and
the public/private redistribution decision.

Prefer CC0-1.0, public domain or Toymoil first-party CC0 content. Do not introduce
NC, ND, SA or ambiguous sources without a prior product decision.

## Flow

```text
discover -> verify license -> save local source -> hash -> select
         -> derive -> visual review -> publish decision
```

Downloaded packs, references, candidates and caches stay under .local. Only the
used, reviewed, traceable outputs may enter public content.
