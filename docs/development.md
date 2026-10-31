# Development and source verification

This repository originally contained only index.html and privacy.html. There is
no package manifest, dependency install, generated build, application test suite,
server or launchd job. Edit the self-contained HTML only under the approved public
content scope; ordinary docs changes need no site build or runtime restart.

## Static checks

- Inspect Git status/diffs before edits and preserve unrelated work.
- Validate Markdown relative links/fences/whitespace, including sibling references
  from the deeper docs directory. External links require separate network checks.
- Verify HTML local links: homepage privacy.html and privacy page ./ navigation.
- For documentation-only work compare both HTML hashes to the starting baseline.
  Do not present successful hashes as live-site/browser/OAuth evidence.
- Preserve existing page title/meta/style/content and policy date unless those are
  the requested change. No automatic legal/privacy wording rewrite or new framework.

Browser rendering or live HTTPS inspection is a separate useful check when HTML
changes. Neither requires login, mail/Keychain access or opening a Google consent
flow. Do not run the private connector's test suite/setup here; it is a different
project and some connector paths access real mail.

## Publication/privacy

This repository is public and main/root is the Pages source. Every file added
should be safe to publish, including agent instructions and Markdown. Do not put
private TODOs, OAuth client JSON, tokens, account mappings or mail evidence here.
No secrets were accessed or stored as part of documentation setup. See
[Publishing](publishing.md) before any separately approved commit/push/settings change.
