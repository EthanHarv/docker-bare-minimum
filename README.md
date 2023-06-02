# Docker Compose with Github Actions

## The Bare Minimum

A lot of docker demos have a bunch of irrelevent files that clutter up the demo.
I wanted to create one with as little as possible to show the absolute bare minimum needed for a simple process.

## Requirements

1. If using Actions, create a Github Personal Access Token with `write:packages`, `read:packages`, and `delete:packages` along with `repo` and `user`
    - Settings -> Developer Settings -> Personal Access Tokens -> Tokens (classic)
2. In your repository, add it as an actions secret with the name `GHCR_TOKEN`
3. Change all mentions of "ethanharv" to your github username, in all lowercase.
    - (`docker-compose.yml` and `.github/workflows/do_docker_things.yml`)

## Running

The action will be run immediately upon push.

For "development," run `docker compose -f docker-compose.dev.yml up`

For "production," run `docker compose up`
