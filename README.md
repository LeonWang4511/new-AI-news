# Agent Workspace · Interactive Preview

**Current release:** `3.0.2`  
**Live site after GitHub Pages activation:** https://leonwang4511.github.io/new-AI-news/

The current release is served from [index.html](./index.html).  
The immutable snapshot is [releases/3.0.2/index.html](./releases/3.0.2/index.html).

## GitHub Pages initial setup (one time only)

In repository **Settings → Pages**:
- Build and deployment → Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/ (root)**
- Save

Public repository / GitHub Free: no paid hosting or custom domain is required.

## Version discipline

Every code/design change requires a higher unique version number.
Do not overwrite an archived release.
For each release, save its immutable HTML at `releases/<version>/index.html` and update the root `index.html` to that exact version.
The root file is the only live publishing entry point.

## Scope

This is an interactive local frontend prototype using browser storage. It does not connect to Windows, Claude Code, Codex CLI or real agents, and does not require credentials or model APIs.
