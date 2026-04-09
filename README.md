# Zeckit Project

This repository currently contains **GitHub Actions automation** for running **ZecKit E2E CI**.

## What’s included

- **E2E workflow**: `.github/workflows/zeckit-e2e.yml`
  - Triggers on pushes / pull requests to `main` and `master`, and can be run manually.
  - Starts a **ZecKit Devnet** using the `intelliDean/ZecKit` GitHub Action (backend: `zaino`).

## Running the workflow

- **On PR / push**: open a PR (or push) to `main`/`master` and GitHub Actions will run automatically.
- **Manually**: in GitHub, go to **Actions** → **ZecKit E2E CI** → **Run workflow**.

## Customizing

Edit `.github/workflows/zeckit-e2e.yml` to change:

- **Devnet backend**: `with.backend`
- **Startup timeout**: `with.startup_timeout_minutes`
- **Branches**: `on.push.branches` / `on.pull_request.branches`


## License

Add a `LICENSE` file if you plan to publish or share this repository.

