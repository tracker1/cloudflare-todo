# Developer Documentation

This document applies to Humans and AI Agents. It should be used and updated
as a core reference for the project details.

## Source Code

Please use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
for all commit messages.

## Development logs

You should track progress under `dev-logs/` in the project root when working
through issues/changes and construction. This goes beyond the git logs, and
all agent prompts and interactions should be tracked in these logs as well.

Under the `dev-logs/` each date whould have a `YYYYMMDD.md` corresponding
file, create if it doesn't exist. Each general interaction should be tracked
as an H2 heading (`##`), where agents should capture the literal prompt as well
as a very terse sumary of the logic/thinking/result made.

Tip: You can run the following command on the CLI in order to get the
timestamp to use or the H2 heading.

```
 deno eval "console.log(new Date().toJSON())"
```

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
