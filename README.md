# SchoolBrief Roadmap

This public repository tracks user-visible SchoolBrief bugs, feature requests, district requests, known limitations, and planned improvements.

SchoolBrief's production source code and internal engineering investigations are maintained separately. This repository is intentionally written for users and may also be used as a public data source for `schoolbrief.io`.

## What belongs here

- Confirmed user-visible bugs
- Feature requests
- Requests for additional school districts
- Known limitations worth communicating publicly
- Planned improvements and release-oriented roadmap items
- Public explanations of why selected work matters

## What does not belong here

Do not post security vulnerabilities, credentials, private information, internal provider details, exploit instructions, or production diagnostics in a public issue.

For a security concern, use the private contact process described in [SECURITY.md](SECURITY.md).

## Public issue structure

Curated SchoolBrief roadmap items should explain more than a title and status. When an internal item is deliberately promoted here, the public version should normally include:

- **Description** — what SchoolBrief plans to fix, add, investigate, or communicate.
- **Why this matters** — the family/user/product reason the work is worth doing.
- **Origin / source** — a public-safe explanation of how the item entered the roadmap, such as user feedback, district onboarding, product roadmap, an observed limitation, App Store requirements, or another public issue.
- **What completion means** — the user-visible outcome and, when relevant, the verification layer required before SchoolBrief calls it released.

Internal engineering issue text is never copied here automatically. Private incidents, provider behavior, security mechanics, diagnostics, budgets, and exploit-relevant details remain private.

## Status language

Public issues should use clear status language such as:

- **Under review** — the request or report is being evaluated.
- **Planned** — SchoolBrief intends to address it, but timing may not yet be committed.
- **In progress** — implementation work is underway.
- **Verification** — a change exists but the intended released/runtime behavior has not yet been fully confirmed.
- **Released** — the change has been delivered at the stated verification layer.
- **Not planned** — SchoolBrief does not currently intend to implement the request.

A source-code change is not automatically described as released. Public status should reflect the strongest layer actually verified.

## Website integration

This repository is designed so its public information can later appear directly on `schoolbrief.io` without exposing private engineering data.

The website can use any of three approaches without restructuring this repository:

1. Link directly to the GitHub issues and roadmap.
2. Fetch public GitHub issues during a static website build and render them on a SchoolBrief roadmap page.
3. Consume the stable, repository-hosted public data contract in [`public/roadmap.json`](public/roadmap.json).

The JSON contract is intentionally presentation-neutral so the website is not coupled to GitHub's page layout. Version 2 includes public-safe `description`, `why`, and `origin` fields, plus optional provenance detail/source URLs when the supporting source itself is public.

The JSON file must never contain private issue text or internal implementation details.

## District requests vs. missing sources

A **district request** asks SchoolBrief to support a district or area that is not currently part of the product.

A **missing school source** means SchoolBrief already supports the school/district but a useful public source is absent or needs review. Those belong in the SchoolBrief source-submission experience rather than being treated as geographic expansion requests.

## Unofficial service

SchoolBrief is an independent service and is not affiliated with or endorsed by the school districts whose public information it organizes.
