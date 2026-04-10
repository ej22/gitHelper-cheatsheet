# git.how — Git & GitHub CLI Cheat Sheet

A single-page, self-hosted reference for Git and the GitHub CLI (`gh`). Served via Docker + nginx.

## Features

- Covers Setup & Config, Staging & Commits, Branching & Merging, Remote & Sync, Stash & Clean, History & Inspection, Undoing Things, Tags & Releases, GitHub CLI, `.gitconfig` Tips, and GitHub Actions Basics
- Light/dark mode toggle
- Sticky nav bar with jump links to each section
- Static HTML — no build step, no dependencies

## Running locally

```bash
docker compose up -d
```

The site will be available at [http://localhost:8167](http://localhost:8167).

## Project structure

```
.
├── docker-compose.yml   # nginx:alpine container, port 8167
├── nginx.conf           # gzip, caching, and security headers
└── src/
    └── index.html       # entire app — styles, content, and JS in one file
```

## Stopping

```bash
docker compose down
```
