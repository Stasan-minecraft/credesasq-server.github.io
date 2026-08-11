# Sensar Translate Update Server

Stable channel for Sensar Translate.

- `manifest.json` is the client-visible release manifest.
- `payload/SensarTranslate-update.zip.b64.part01.txt` ... `part07.txt` contain the Base64-encoded update ZIP.
- The client reconstructs the ZIP locally, validates `zip_sha256`, extracts `SensarTranslate.exe`, validates `sha256`, waits for the running process to exit, replaces it, and restarts.
- Current stable build: 4.0.0 (400).

Do not change hashes without publishing matching payload parts.
