# GitHub API /meta Log

Automated hourly snapshots of [https://api.github.com/meta](https://api.github.com/meta), committed to this repository so that every change is captured in the Git history.

## How it works

A GitHub Actions workflow runs every hour (and on manual trigger):

1. Fetches the current JSON from `https://api.github.com/meta`
2. Pretty-prints it to `meta.json`
3. Commits and pushes only if the content has changed

Browse the [commit history of meta.json](../../commits/main/meta.json) to see all recorded changes.
