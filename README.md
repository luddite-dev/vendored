# Vendored Binaries

This repository manages the build pipeline for vendored binaries used by Luddite.

## Artifacts

### Caddy

Custom Caddy build with the `caddy-dns/cloudflare` plugin baked in.

- **Manifest:** `manifest.json` tracks the latest version, checksums, and download URLs.
- **CI:** Daily check for new upstream Caddy releases. Builds and publishes automatically.
- **Consumers:** Periphery fetches `manifest.json` to detect version changes and auto-updates the local binary.
