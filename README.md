# scholarly-gateway-mcp — Integration Proof Artifact

This repository is a minimal, known-good integration artifact for:
- **scholarly-gateway-mcp** (V1 contract frozen, deterministic)

It exists to reduce integration friction for strangers:
- show exactly what to run
- show exactly what to send
- show what to capture for bug reports (including `provider_status`)

## What this proves

- Installation works from PyPI
- The MCP server can be started
- A client can call tools using **exact JSON payloads**
- Responses include `provider_status` needed for structured bug reports

## Known-Good Version

Pinned for reproducibility:

- `scholarly-gateway-mcp==0.2.1`

See also:
- V1 contract: `docs/V1_CONTRACT.md` in the main repo
- Structured bug reporting: use the Bug Report form in the main repo

---

## Quickstart (Local)

### 1) Create and activate a venv

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -U pip
pip install -r requirements.txt
