# Agent Context

for general project constructs that apply to human and AI Agent contributors,
please see and reference the developer documentation under `docs/dev/`,
this file is additional context that should apply to agents specifically.

The main `README.md` file will provide additional project context.

This file may be ammended/updated to save additional contextual details within
the project itself.

## Workflow

### Git Context

While working, there will generally be an "in progress" commit that is ammended
to until a given piece of work is completed. In practice this will be
merged/rebasd witht the main branch at that point. It may be in a working
branch or in the local main branch directly as this is a single-developer
project currently.

### Rollback

While interacting with the project and capturing work. It will sometimes be
necessary to rollback the work to the last commit. The `dev-logs/` directory
should not be rolled back... what should happen is a log entry is added as an
H2 with the timestamp, and noting the rollback.

### Working

Use `dev-logs/` in order to capture the history of events that are using AI to
interact with this project. For each interaction with AI, I would like to add
a `log-YYYYMMDD.md` for every calendar date, if a file for the given date is
not yet created, you should create one.

When the prompt is made, an H2 Heading (##) should be added for the timestamp
(ISO-8601 style in UTC, matching JSON ddefault serialization)
that will contain two sections underneath them. An H3 for the prompt, and
another for the Context/AI process and results from the work as a bulletted
summary... the main point is to capture the prompt itself... the results from
the work may be summarized.

Further interactions should ammend a new H2 heading for the timestamp and the
next prompt.

### Commit

When reaching a "good" intersticial point, the work should be captured/ammended
to the working commit in order to preserve the current status. The agent log
should be ammended before commit noting the save point.
