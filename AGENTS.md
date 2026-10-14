# Working in this repository

Instructions for any AI agent or contributor working on dark-project:
a dark-themed game landing page.

## Start here

Read these, in order. Do not load the whole `docs/` folder — read only what
your task needs.

1. This file.
2. [`docs/explanation/constraints.md`](docs/explanation/constraints.md) — the
   realities that make the usual way wrong here.
3. The issue or plan you are working on.

## Do and don't

| Rule | Why |
|---|---|
| Branch fresh from `main` for every change. | Old branches carry other people's unmerged work. |
| Never force-push or rewrite pushed history. | Others may have built on it. |
| Never commit a secret or a `.env` file. Add new variables to `.env.example` with a safe placeholder. | A pushed secret is public forever, even after deletion. |
| No AI attribution in commits or pull requests: no `Co-Authored-By` naming an AI, no "Generated with" line. | Commits are the human contributor's record. A hook and CI enforce this. |
| Only ikkeflikkeri merges pull requests. | The owner decides what ships. |
| [OWNER: what must never happen? (Q7 was "idk")] | — |

## Imitate

Read one of these and copy its shape. This is faster and more reliable than
any description.

| Writing | Copy the shape of |
|---|---|
| [OWNER: which file shows the right way to write a page or component?] | — |

## Verify before reporting done

Run these. Do not report work done on the basis that it looks right.

```
[OWNER: how do you run the typecheck?]
[OWNER: how do you run the lint?]
[OWNER: how do you run one test file?]
```

CI runs the full test suite. Locally, run only the tests for the files you
changed.

## Where it runs

- Staging: there is no staging.
- Production: [OWNER: where does production run?]
