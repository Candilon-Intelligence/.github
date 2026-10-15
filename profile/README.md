# Candilon Intelligence

**Trusted data before trusted AI.**

Candilon builds governance infrastructure for AI in organisations that handle sensitive data, starting with health and education in Africa.

## What we are building

**Data plane.** Takes a tabular dataset through cleaning, PII discovery (structured fields and free text), de-identification by policy, privacy-risk measurement with ARX (k-anonymity, uniqueness, re-identification risk), quality checks, and a named human approval gate. Every stage is recorded in a hash-chained provenance log.

**AI plane.** Answers questions only from approved data. A rule-based router selects language, domain and expert slot. Counts and averages are computed from tables rather than generated. Other questions use keyword retrieval over documents. Each answer is verified against its evidence and is labelled GROUNDED, PARTIAL, UNSUPPORTED or ABSTAINED. When there is no evidence, the system declines to answer.

Both planes run locally in Docker, and can also run on Google Colab for demonstrations.

## Status

This is an early prototype. It has been tested on synthetic data. It is not yet deployed at any institution, and it does not yet include sign-in, role-based access, encryption at rest, or a formal security review. Models currently used are general open-weight models; domain adapters are planned, not built.

## Principles

- Raw sensitive data is cleaned, measured and approved before any model uses it.
- Institutions keep control of their data and can see what was used.
- Every answer shows its evidence and its verification status.
- Models are replaceable settings, not the product.

## Roadmap

- Sign-in, roles and access tiers
- Output labelling and signed provenance records
- Domain adapters trained on approved, de-identified data, with evaluation on held-out test sets
- Pilot deployments with partner institutions under written data-sharing agreements

## Get in touch

Website: candilon.com
Contact: candilon.intelligence@candilon.com
