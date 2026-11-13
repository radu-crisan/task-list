# Development environment

How to start the project. This is the page the agent must find when asked
"how do I start the project?".

Write commands exactly as they are typed. If a command differs on Windows,
give both versions.

## Requirements

Docker with Compose and Git. Node 24 and Yarn 4 (via corepack) exist only in
the image built from .docker/; do not install them on the host.

## Start

```
docker compose up -d --build
```

The container `app` stays running in the background with the project mounted
at /app. Address of the dev server, once Vite is set up: http://localhost:5173
(the port compose.yaml publishes).

## Stop

```
docker compose down
```

## Run a command

Node and Yarn run only in the container, through `docker compose exec app`:

```
docker compose exec app yarn install
docker compose exec app yarn <script>
```

Use `docker compose exec -T app ...` in scripts without a terminal.
package.json has no scripts yet.

## Common problems

None recorded yet.
