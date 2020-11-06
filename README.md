# sqlite-practice: a containerized SQLite playground

## ([Click Here To Check Out This Repo's Landing Page](https://asa55.github.io/sqlite-practice/))

<img alt="SQLite Logo" src="img/sqlite-logo.svg" width="30%" />

## Wondering what this repository is for?

I wanted to play around with [SQLite using this tutorial](https://sqlite.org/cli.html). But I don't like installing programs directly on my computer (un-installing every last file isn't always straightforward). Containerizing SQLite (as this repo does) avoided this problem entirely.

By following the steps below, we can spin up a local SQLite engine inside a container and play around with the CLI (from inside the container). SQLite databases are just .db files that live in a filesystem. There aren't any special processes you need running in the background to keep it alive - all it needs fo function are the typical filesystem ops. The steps below will create a SQLite DB on your local filesystem, but everything else we need to manipulate it will live inside a container (for easy teardown after we're done playing around).

## Here's how to use this repo to practice with SQLite locally:

1. Clone the code to a local folder on your machine

2. Open in container with VSCode remote container extension (requires Docker)

3. Run the following command from inside the container (persists in host OS storage volume):
```sqlite3 test.db```
