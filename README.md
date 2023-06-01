# Docker w/ Actions

## The bare minimum

A lot of docker demos have a bunch of irrelevent files that clutter up the demo.
I wanted to create one with as little as possible to show the absolute bare minimum needed.

## Requirements

// TODO

1. Create a github Personal Access Token with `write:packages`, `read:packages`, and `delete:packages` along with `repo` and `user`
    - Settings -> Developer Settings -> Personal Access Tokens -> Tokens (classic)
2. In your repository, add it as an actions secret with the name `GHCR_TOKEN`
