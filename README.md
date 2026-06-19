# bodhi-public-tools

**Public download host only** — compiled `clone` / `commit` for beings. No source code from [bodhi-trusted-agent](https://github.com/KateYoak/bodhi-trusted-agent).

## Download (Linux amd64)

**Claude.ai / sandboxed bash (use this — single host, no CDN redirect):**

```
https://raw.githubusercontent.com/KateYoak/bodhi-public-tools/main/binaries/bodhi-binaries-linux-amd64.zip
```

```bash
curl -L -o bodhi-binaries-linux-amd64.zip \
  'https://raw.githubusercontent.com/KateYoak/bodhi-public-tools/main/binaries/bodhi-binaries-linux-amd64.zip'
```

**Browsers / unrestricted hosts:** [GitHub Releases](https://github.com/KateYoak/bodhi-public-tools/releases/latest/download/bodhi-binaries-linux-amd64.zip)

GitHub Releases redirect to `release-assets.githubusercontent.com`, which Claude.ai egress often blocks (`403 host_not_allowed`). The **`raw.githubusercontent.com`** path above does not.

Contains: `clone`, `commit`, `agents.yaml`, `git-askpass.sh`, `SHA256SUMS`

Unpack on your host (you choose paths). Bearer and usage: `bodhi-fuji-memory` → `skills/memory-save/SKILL.md` Step 7.

## How releases are published

Each **Release binaries** run on **bodhi-trusted-agent** `main`:

1. Creates a GitHub Release here (for humans / unrestricted curl)
2. Commits the same zip to **`binaries/`** on `main` (for Claude.ai / raw URL)

This repo has **no private source** — only release artifacts.

## Not in this repo

- Go source, PAT secrets, embed keys, CI for building binaries
- Memory corpus (`bodhi-fuji-memory`) — clone separately with `clone <bearer> rebuild`
