# Contributing to SwitchStone

Thank you for contributing to SwitchStone. This document outlines our development workflow, patch standards, and expectations across all `switchstonedev` repositories.

## Contributing Patches

1. **Single-Purpose Patches:** Break work into small, single-purpose pull requests whenever possible. Large diffs with disjoint changes are significantly harder to review, test, and benchmark.
2. **Propose Major Changes First:** For non-trivial architectural modifications, new benchmark suites, or breaking API changes, open an issue to discuss design and scope before writing code.
3. **Fork and Branch:** Fork the target repository and create a dedicated feature branch from `main`. Use descriptive branch prefixes (`feat/...`, `fix/...`, `perf/...`, `docs/...`).
4. **Pull Request Naming:** Prefix your PR title with the relevant component or Conventional Commit tag:
   - `[VectorDB] Add HNSW recall@k evaluation pipeline`
   - `[CPRecommender] Fix rating decay calculation in CF model`
   - Or standard Conventional Commits: `feat(vectordb): ...`, `fix(cprecommender): ...`
5. **Testing and Verification:**
   - Make sure all existing unit tests, integration tests, and benchmarks pass locally.
   - Add new automated tests for any new functionality or bug fixes.
   - Verify code formatting and linter checks pass with clean exit codes.
6. **PR Description & Transparency:**
   - Fill out all required sections in the pull request template: **Rationale**, **Changes included**, **Test verification**, and **User-facing changes** (breaking changes or critical fixes).
   - Disclose AI-generated assistance in accordance with our transparency checklist.

## Reporting Bugs and Enhancements

- **Bug Reports:** Use the structured Bug Report form under `.github/ISSUE_TEMPLATE`. Include reproducible code snippets, error output, version/commit hash, and select the affected component(s).
- **Enhancement Requests:** Use the Enhancement Request form to detail the problem statement, proposed solution, and affected component(s).
- **Discussions:** For broader architectural questions or benchmark methodology inquiries, join our community discussions.

## Code Review

All submissions are reviewed by the maintainer. Keep pull requests focused on a single change set with concise diffs to facilitate prompt review.
