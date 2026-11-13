# Task List

To-do web app with accounts, tasks and administration. Front end only for now
(Vue + Vite + Tailwind); there is no API. Today's scope is the login page.

## Non-standard
- Everything runs in Docker (compose.yaml, node 24); Yarn 4 with node_modules.
- Node and Yarn exist only in the container: `docker compose exec app yarn ...`.
- No API: login is simulated in the front end.
- Never set up Vite, Vue or Tailwind unasked; the human does it.

## Structure
src/ front end · docs/ project memory · bin/ checks · .docker/ image

## Where to look
- docs/state.md: first, in every session
- docs/hard-rules.md: before you change any file
- docs/dev-environment.md: how to start the project
- docs/testing.md: before you say something works
- docs/architecture.md: before you add a module or change how parts connect
- docs/conventions.md: before you write code or commit
- docs/workflow.md: before you open a pull request or release
- docs/decisions.md: before you reopen a decision
- docs/specs/: the spec, before you build anything
- docs/mockups/: visual references, not specs
- docs/ai-log.md: the human's own AI log; read it, never edit it
