# Developer Documentation

This document applies to Humans and AI Agents. It should be used and updated
as a core reference for the project details.

## Source Code

Please use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
for all commit messages.

## run/ scripts

[run](run/index.md) scripts will be used in order to exercise and orchestrate
things within the application for developer runtime usage, testing and even
to aid build and deployment or other tasks.

## Testing

When running tests, prefer to run full suite checks via `run/test` or similar
in order to establish that full context and workflows actually work instead
of running specific singular tests, or directly testing functionality.

## Structure

This is a mono-repo which contains application sources for several projects
that will work together as a final solution. Each project section will be
under `projects/$NAME` and will have its' own README as the project evolves.
