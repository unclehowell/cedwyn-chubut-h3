# Chubut H3

The Chubut H3 map webapp of [cedwyn.bucklerfamily.estate](https://cedwyn.bucklerfamily.estate/chubut-h3/), in its own repository.

Split out of `unclehowell/cedwyn` (branch `section/chubut-h3`) as part of REPO SPLIT (issue #188). That repository holds hundreds of branches; a job on one webapp should never need the rest.

## Get the code

```
git clone --depth 1 https://github.com/unclehowell/cedwyn-chubut-h3.git
```

## Where to send changes

The current `split-repos.json` entry in `unclehowell/cedwyn` sets this app to `mode: split-repo`. **This repository's `main` branch is the source of truth.**

1. Make application changes on a feature branch in this repository.
2. Open a pull request into this repository's `main`.
3. After merge, Cedwyn's scheduled `sync-split-repos` workflow copies `main` into the retained legacy branch `section/chubut-h3`.
4. The central `build-cedwyn` workflow assembles the unified site from the synced branch.

Do not open application pull requests against the legacy branch `section/chubut-h3`; it is a compatibility mirror, not the development target. Site-wide registry, shared runtime, central catalogue and build changes still belong in `unclehowell/cedwyn` `main`.

Full instructions: [REPO-SPLIT.md](https://github.com/unclehowell/cedwyn/blob/main/docs/REPO-SPLIT.md).


## History before the split

https://github.com/unclehowell/cedwyn/commits/section/chubut-h3

Never force-push; never delete the old branch.
