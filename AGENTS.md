# AGENTS.md

Guidance for coding agents working in this repository. Humans: see [README.md](README.md#contributing).

## What this is

Complete Bever models. Each folder has `bev/*.bev` and a `README.md` saying what it demonstrates and how to try it.

## Read first

| Topic | Document |
| --- | --- |
| Language | [bever.dev/reference/language](https://bever.dev/reference/language) (`../bever.dev/docs/reference/language.md` when checked out alongside) |
| Guides | [bever.dev/guide](https://bever.dev/guide/what-is-bever) |

## Commands

```sh
bever check <example>/bev     # must pass for every example; CI checks all of them
```

## Rules

- Use only implemented language. Planned features from the roadmap do not compile.
- Add an example only when it shows something the others do not, and list it in the README table.
- Examples that the bever.dev tutorial or guides use must stay in sync with those pages.
- Use neutral names (Ada, Bob) and `example.com` addresses.
