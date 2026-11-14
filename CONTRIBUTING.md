# Contributing to SwitchStone

Thank you for contributing to SwitchStone projects. This document outlines the standard development workflow and expectations across all `switchstonedev` repositories.

## Workflow

1. **Fork and Branch:** Fork the target repository and create a dedicated feature branch from `main`. Use descriptive branch prefixes:
   - `feat/<short-name>`
   - `fix/<short-name>`
   - `docs/<short-name>`
   - `perf/<short-name>`
   - `chore/<short-name>`
2. **Propose Major Changes First:** For non-trivial features or architectural modifications, open an issue to discuss design and scope before writing code.
3. **Commit Standards:** Use [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` new capabilities or interfaces
   - `fix:` bug fixes
   - `perf:` performance improvements
   - `docs:` documentation updates
   - `chore:` maintenance tasks or dependency updates
   - `ci:` workflow or CI configurations
4. **Testing and Linting:** Run relevant test suites and linters locally before submitting. Ensure:
   - All existing and new unit/integration tests pass.
   - Code adheres to the repository's formatting and linting rules.
   - Any added behavior includes corresponding automated test coverage.
5. **Pull Request:** Open a pull request against the `main` branch. Complete the provided PR template checklist. If the PR is a work in progress, mark it as a draft.

## Code Review

All submissions are reviewed by the maintainer. Keep pull requests focused on a single change set with concise diffs to facilitate prompt review.
