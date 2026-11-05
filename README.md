# cloudflare-todo

This is a simple demonstration application using Cloudflare services, in
particular a web-worker for the web services, connecting to D1 and a voice
agent for the purpose of managing a simple TODO list.

- UI: React, Zustand and Mantine
- API: Hono
- Cloudflare Worker: Serve UI and runs API
- Cloudflare D1: Data storage for simple auth and todo lists
- Cloudflare Voice Agent: to manage the TODO list with a voice interface

A portions of this project will be developed with the use of an AI agent,
in particular Claude Code (Opus 5.5). Prompt history should be captured
through log files under `agents/`.

# Documentation

Documentation will be split under `docs/` depending on the context.

- [Developer Documentation](./docs/dev/index.md) for contributors (Agent and Human).
- [Operator Documentation](./docs/ops/index.md) for running and deploying the apps.
- [User Documentation](./docs/user/index.md) for users interacting with the UI/UX.

# License

Copyright © 2026 Michael J. Ryan <tracker1@gmail.com>

[ISC License](LICENSE.md).
