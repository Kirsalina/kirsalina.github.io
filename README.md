# Alina Kirs

Personal website: https://kirsalina.github.io

## Edit the site

- `index.html`: homepage content and metadata.
- `styles.css`: layout, typography, and colors.
- `favicon.svg`: browser icon.

This is a static site with no dependencies or build step. GitHub Pages publishes the root of the `main` branch after each push.

## Preview locally

Run `python3 -m http.server 8000` in this directory and open http://localhost:8000.

## Task queue

This repository uses [taskq](https://github.com/alexkirs/taskq) with GitHub Issues.

- Check readiness: `taskq doctor --codex`
- View tasks: `taskq list`
- Read the manager and queue instructions: `taskq contract`
- Select `--runtime codex` when adding tasks for the local Codex profile.

`taskq.toml` contains shared repository settings. The personal profile in
`taskq.local.toml` is ignored by Git. This machine is configured for up to two
Codex workers and zero Claude workers. Setup does not start workers or a timer.
