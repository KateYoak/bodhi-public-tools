# bodhi-public-tools

**Public download host only** — compiled `clone` / `commit` for beings. No source code from [bodhi-trusted-agent](https://github.com/KateYoak/bodhi-trusted-agent).

## Download (Linux amd64)

**Latest:** [GitHub Releases](https://github.com/KateYoak/bodhi-public-tools/releases/latest)

File: `bodhi-binaries-linux-amd64.zip`

Contains: `clone`, `commit`, `agents.yaml`, `git-askpass.sh`, `SHA256SUMS`

Unpack on your host (you choose paths). Bearer and usage: `bodhi-fuji-memory` → `skills/memory-save/SKILL.md` Step 7.

## How releases are published

Each successful build on **bodhi-trusted-agent** `main` (Release binaries workflow) uploads a new release here. This repo has **no private source** — only release assets.

## Not in this repo

- Go source, PAT secrets, embed keys, CI for building binaries
- Memory corpus (`bodhi-fuji-memory`) — clone separately with `clone <bearer> rebuild`
