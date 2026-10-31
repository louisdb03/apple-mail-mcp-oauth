# GitHub Pages publishing

## Observed configuration

Read-only repository/Pages API discovery during this documentation pass returned:

- Repository louisdb03/apple-mail-mcp-oauth, public; default branch main.
- Pages URL https://louisdb03.github.io/apple-mail-mcp-oauth/.
- Pages source main at / (repository root), build_type legacy, status built.
- Local remote origin points to that repository over SSH.

This is the observed configuration, not a fresh rendered-site/content comparison.
The pass did not push, change Pages settings or edit the existing HTML. The
Pages build_type label describes GitHub hosting, not retirement of this project.

## Approval and verification

1. Review exact public diff and candidate filenames for private data/secrets.
   This is not a private operational notebook; main/root can serve added files.
2. Obtain approval before commit/push or Pages/Google OAuth configuration changes.
   Do not assume documentation approval includes public publication.
3. After an approved push, read exact remote branch SHA and compare local HEAD.
   Read Pages build/status independently; a successful push alone is not deployment.
4. Fetch actual homepage/privacy URLs with normal TLS verification and compare
   intended titles/content/links. Where layout changed, inspect browser rendering
   and narrow/light/dark behaviour separately from HTTP status.
5. Report Git publication, Pages build and served-content checks separately. No
   email access or live OAuth sign-in is needed to prove static content deployment.

The GitHub Pages URL is not an implemented redirect URI/callback endpoint. Google
Cloud consent/client settings and the desktop connector's credential storage are
owned elsewhere; don't change app publishing state, grants, scopes or credentials
to make this static site check pass. No DNS/custom-domain or backend migration is
part of this documentation task.
