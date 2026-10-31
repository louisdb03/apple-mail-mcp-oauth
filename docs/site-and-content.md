# Site structure and content ownership

## Implemented pages

| Source | Content |
| --- | --- |
| index.html | Personal-use Apple Mail MCP description, privacy link and contact mailto |
| privacy.html | Stated Gmail operations/data handling, Google API policy/Limited Use, revocation and contact/home links |

Both are self-contained semantic HTML with embedded CSS, UTF-8, responsive viewport,
640px content width, system fonts and light/dark colour scheme. No JavaScript,
tracking, cookies, external font/script library, form or API handler is implemented
in this checkout. GitHub/Google/browser infrastructure has its own behaviour;
source simplicity is not a claim about every hosting/request log.

The privacy page's displayed last-updated date is 25 October 2026. Do not bump it
for internal documentation work that did not change the policy. Keep homepage/
privacy links relative so the repository-nested Pages path works. Google policy
and revocation links are external navigation, not local auth implementation.

## Public claims versus runtime guarantees

The HTML describes a personal tool for the owner's Gmail account, limited message
lookup/label operations, local Keychain sign-in, and no content reading/sending/
deletion through that intended Gmail path. It states data-use and Limited Use
commitments. This repository implements none of the underlying mail behaviour.
Preserving these words does not certify their continuing accuracy or compliance.

The separate connector's Gmail documentation describes more detailed folder/label
operations and broader gmail.modify privilege. A scope can exceed the intended
code path; consent is not approval for every possible Gmail action. Current public
claims should be reviewed against actual connector code before a separately
approved release that changes behaviour. This docs pass did not perform a full
privacy/code audit or revise the published policy.

## Integration ownership

[Apple Mail MCP](../../apple-mail-mcp/README.md) owns server/API behaviour, Gmail
setup and Keychain helper. Its [Gmail reference](../../apple-mail-mcp/docs/gmail.md)
is local/private development guidance, not publicly linked support content for
site visitors. Google owns consent/client configuration and account revocation;
GitHub Pages owns public static hosting. No credential exchange/callback service
runs here. Do not copy setup secrets or private connector internals into public
docs to explain this relationship.
