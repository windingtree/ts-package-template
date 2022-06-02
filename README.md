---
author: mfw78 <mfw78@protonmail.com>
---

# WT Typescript / Javascript Repo Template

## Overview

This is a template repository to be used for `node.js` and browser-based package / project development. This repository contains the base tools required for linting, building, packaging and deploying to `npmjs`. Tools used include:

- eslint
- prettier
- git-cz
- conventional commits
- typescript
- dotenv

## Commits

To commit to the repository after staging the files for commit:

```bash
yarn commit
```

Select the appropriate type of commit message, any issues to close, and note any breaking changes.

**Note**: This will enforce _conventional commit messages_ and _GPG signatures_ on commits.

**Note**: `commitlint` is enabled within the repository so all commits that do not abide by `conventional commits` will be rejected, as `semver` relies on this.

## Deployment

Automatically publishes according to `semver`. Publishes to `npmjs` when a `PR` is pushed into the `main` branch.