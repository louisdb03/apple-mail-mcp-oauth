# Apple Mail MCP OAuth site — agent instructions

## Scope

This repository is a small public static homepage/privacy-policy site for the
personal Apple Mail MCP OAuth client. It is **not** an OAuth server, callback
handler, Gmail API implementation or mail-processing service. The actual connector
and credential/setup logic live in ../apple-mail-mcp, whose guidance must be read
explicitly before work there. Do not move client secrets/tokens/account mappings
or real mail into this public repository.

README.md is user-facing; docs/index.md links ordinary shared reference. Keep
agent instructions in root CLAUDE.md for Hermes/Claude Code. Linked files require
an explicit read; no automatic parent/project instruction inheritance is assumed.

## Files and ownership

- index.html: public description and privacy/contact link.
- privacy.html: public data-use/privacy statements and Google policy/revocation links.
- docs/site-and-content.md: actual static design and content/implementation boundary.
- docs/development.md: local source checks and no-build workflow.
- docs/publishing.md: verified Pages configuration and separate publication gate.
- ../apple-mail-mcp/docs/gmail.md: connector-owned OAuth setup/scopes/Keychain details.

## Safety and change boundaries

Inspect Git status/diffs and preserve existing work. This is a public repository,
with GitHub Pages sourced from main at repository root. Treat all committed files
as potentially published; Markdown is not a private notes area. Never include
credentials, downloaded OAuth JSON, tokens, private identifiers/messages or logs.
Local cross-repo links are development references, not guaranteed public URLs.

Leave public HTML/privacy statements unchanged unless that content revision is
explicitly authorised. Policy assertions are not independently verified runtime
facts; check current connector code and actual scope before proposing revisions.
Do not silently broaden personal-use claims, promise legal compliance, change
contact details or claim Gmail scope itself enforces code-level restrictions.

The public site does not authenticate anyone or store tokens. Gmail OAuth consent
and runtime credential handling belong to Google/the private connector, not Pages.
No JavaScript/API/backend/build manifest is present. Do not add an OAuth callback,
analytics, forms, remote scripts or dependencies as documentation housekeeping.

## Verification/publication

For docs-only edits check relative links, fences/whitespace, baseline HTML hashes
and Git diff; no mail/Keychain access, Google Cloud changes or OAuth flow needed.
Never invoke connector tests/setup merely to document this site.
Commit/push/Pages settings and public content changes need explicit approval.
Read back remote SHA/Pages status and actual served page content after approved
publication; a successful push or prior built status is not fresh deployment proof.
No service or Hermes restart is needed for these static source/docs changes.
