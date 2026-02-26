# scholarly-gateway-mcp — Integration Proof Artifact

This repository is a minimal, known-good integration artifact for:

- **scholarly-gateway-mcp** (V1 contract frozen, deterministic)

It exists to reduce integration friction for strangers:

- Show exactly what to run
- Show exactly what to send
- Show what to capture for bug reports (including `provider_status`)
- Provide a reproducible Claude Desktop MCP configuration

---

## What this proves

- Installation works from public PyPI
- The MCP server can be started deterministically
- A client can call tools using exact JSON payloads
- Responses include `provider_status` needed for structured bug reports
- Claude Desktop integration works via stdio transport

---

## Known-Good Version

Pinned for reproducibility:

- `scholarly-gateway-mcp==0.2.2`

See also:

- V1 contract: `docs/V1_CONTRACT.md` in the main repo
- Structured bug reporting: use the Bug Report form in the main repo
- Compatibility Matrix: see pinned issues in the main repo

---

## Quickstart (Local)

### 1) Create and activate a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -U pip
pip install -r requirements.txt
