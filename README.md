# apple-docs-wwdc-data

WWDC session data (transcripts, code examples, topics) downloaded on demand by the [Emasoft Apple Documentation](https://github.com/Emasoft/emasoft-apple-documentation-plugin) Claude Code plugin. The plugin fetches the archive from this repository's releases on the first WWDC tool call, verifies its SHA-256, and extracts it into the plugin data folder.

## Releases

- `v2` (immutable, pinned by the plugin): `wwdc-data.tar.gz`, SHA-256 `9e436884c29acb8ccef0b1077bc0713e1d380be513ba174cbf865fa7f17bc3bb`, 10,639,807 bytes.

Releases from `v2` on are GitHub immutable releases. `v1` (same bytes, published before immutability was enabled) is kept only for history. The plugin pins the archive by SHA-256. A data refresh is published as a new release (`v2`, ...) together with a new pin in the plugin.

## Manual install

```sh
mkdir -p <dir> && curl -L https://github.com/Emasoft/apple-docs-wwdc-data/releases/download/v2/wwdc-data.tar.gz | tar xz -C <dir>
```

Then set `APPLE_DOCS_MCP_WWDC_DATA_DIR=<dir>` for the plugin.

## Licence scope

The MIT licence in this repository covers only this repository's own files (this README and the packaging). The archive contents (WWDC session transcripts and code) are Apple's material, redistributed as collected by kimsungwhee/apple-docs-mcp; no licence is granted on them. One sample JWS token in WWDC25 session 221 is redacted.
