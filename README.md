# SchoolBrief Roadmap

This public repository tracks user-visible SchoolBrief bugs, feature requests, district requests, and planned improvements.

SchoolBrief's production source code and internal engineering investigations are maintained separately. This repository is intentionally written for users and may also be used as a public data source for `schoolbrief.io`.

## What belongs here

- Confirmed user-visible bugs
- Feature requests
- Requests for additional school districts
- Known limitations worth communicating publicly
- Planned improvements and release-oriented roadmap items

## What does not belong here

Do not post security vulnerabilities, credentials, private information, internal provider details, exploit instructions, or production diagnostics in a public issue.

For a security concern, use the private contact process described in [SECURITY.md](SECURITY.md).

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
3. Consume the stable, repository-hosted public data contract in [`public/roadmap.json`](public/roadmap.json). That file is intentionally presentation-neutral so the website is not coupled to GitHub's page layout.

The JSON file must never contain private issue text or internal implementation details.

## Unofficial service

SchoolBrief is an independent service and is not affiliated with or endorsed by the school districts whose public information it organizes.
