# Apple Mail MCP OAuth information site

A small **public static site** providing the homepage and privacy policy for
Louis's personal Apple Mail MCP OAuth client.

- Homepage: https://louisdb03.github.io/apple-mail-mcp-oauth/
- Privacy policy: https://louisdb03.github.io/apple-mail-mcp-oauth/privacy.html
- Public source: https://github.com/louisdb03/apple-mail-mcp-oauth

## What this project is—and is not

index.html describes the personal tool and links to privacy.html. The privacy
page explains its stated Gmail use, local credential storage, Google Limited Use
commitment, access revocation and contact route. These are public content claims,
not functionality implemented by this site.

There is no sign-in form, OAuth callback, token storage, Gmail client, mail
processing or backend here. Those belong to the separate
[Apple Mail MCP connector](../apple-mail-mcp/README.md), including its
[Gmail/OAuth reference](../apple-mail-mcp/docs/gmail.md). Those sibling links are
for local development; the connector repository is private and not a public support
resource for site visitors.

## Documentation

| Document | Purpose |
| --- | --- |
| [Index](docs/index.md) | Shared reference navigation |
| [Site and content](docs/site-and-content.md) | Page layout, public claims and connector ownership |
| [Development](docs/development.md) | No-build workflow and source checks |
| [Publishing](docs/publishing.md) | GitHub Pages configuration, privacy and approval boundaries |

Root CLAUDE.md contains shared Hermes/Claude Code agent instructions; README is
the user entry; docs are ordinary reference for both. Keep this project lightweight.
No dependencies/build/server are required to maintain the HTML source.

GitHub Pages configuration was read as main branch / root, build_type legacy and
status built during documentation discovery. This is configuration/status evidence,
not a fresh HTTP/browser test. No HTML, Google settings or published content was
changed by the documentation pass, and nothing was committed/pushed. Publication
of these new files requires separate approval: this repository and its Pages output
are public, so do not add private operational records or credentials.
