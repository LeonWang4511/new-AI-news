# Agent Workspace · Interactive Preview

**Current release: 3.0.3**  
**GitHub Pages:** https://leonwang4511.github.io/new-AI-news/

This repository publishes the root [index.html](./index.html) through GitHub Pages (main branch, root). Version snapshots are immutable:

- [3.0.3](./releases/3.0.3/index.html) — Apple-inspired tactile workspace, floating control materials, actual per-stage visual response, responsive iPad/iPhone layout
- [3.0.2](./releases/3.0.2/index.html) — focused workflow concept

## Release policy

Each change requires a strictly higher unique version number. Never overwrite an archived release. Once a version is complete, save its HTML to `releases/<version>/index.html`, then publish that exact same file to root `index.html`. No manual copying is required from the user after the one-time Pages setup.

## Product scope

This is an interactive local frontend prototype. Planner messages are local mock responses. It does not connect to Windows, Claude Code, Codex CLI, any actual agents, or paid APIs.

## Design references

- [Apple HIG — Materials](https://developer.apple.com/design/human-interface-guidelines/materials)
- [WWDC25 — Build a UIKit app with the new design](https://developer.apple.com/videos/play/wwdc2025/284/)
- [WWDC25 — Elevate the design of your iPad app](https://developer.apple.com/videos/play/wwdc2025/208/)
