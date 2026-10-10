# AGENTS.md

Guidance for AI coding agents working in this repository.

## What this is

`@three-ws/tty-avatar` v0.1.0. A live 3D avatar in your terminal. Renders any GLB (or any three.ws avatar by id) with a software rasterizer to truecolor half-blocks or braille, animates it with moods, and reacts in real time to Claude Code hooks so your coding agent has a face.

A JavaScript library. Import it from ESM.

## Use it

```bash
npx -y @three-ws/tty-avatar
```

Full usage, tool list and configuration are in [README.md](README.md). Machine-readable summaries: [llms.txt](llms.txt) and [llms-full.txt](llms-full.txt).

## Develop

```bash
npm install
npm test
```

Scripts:
- `npm run test`: `node --test test/*.test.js`

## Conventions

- ES modules, Node >=18.
- Read-only by default. Anything that signs, spends or sends must be an explicit, separately named tool or option, and must never be inferred from untrusted text (token names, memos, listings).
- Never commit credentials. Configuration comes from environment variables documented in the README.
- Keep changes small and covered by a test next to the code they change.

## Source of truth

This repository is a generated mirror of `packages` in https://github.com/nirholas/three.ws. Open issues here; send substantial changes as a pull request here or upstream.
