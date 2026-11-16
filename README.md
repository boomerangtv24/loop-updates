# Boomerang Loop updates

Signed update packages for the Boomerang Loop desktop app. Each installed copy reads
`releases/latest/download/manifest.json` and installs a package only if its SHA-256 matches
and Boomerang's Ed25519 signature is valid.

To publish: add `releases/<version>/` with `manifest.json` and `app-<version>.tar.gz`
(made by `desktop/release.sh` in the loop repo) and push to `main`. The workflow creates the release.
