# Run Scripts

This directory will be used for shell scripts and orchestration within this
project. Scripts directly under `run/` will be extensionless and either
Bash or TypeScript. TypeScript scripts will use Deno for the shebang, but
should use the Node API and prefer NPM modules to keep any future migration
easier

- **do not use Deno global or deno-only modules**
- **Do use imports for `node:*` even for pieces that are globals in Node.**

Run scripts will be used in order to exercise and orchestrate things within the
application(s), for developer runtime usage, testing and even to aid build and
deployment or other tasks.

Directories under this one may be mused for extended library or modular reuse
with the scripts themselves.
