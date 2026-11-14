# Contributing to SwitchStone

Thank you for contributing to SwitchStone. This document outlines our development workflow, commit standards, and expectations across all `switchstonedev` repositories.

## Contributing Patches

1. **Single-Purpose Patches:** Break work into small, single-purpose pull requests whenever possible. Large diffs with disjoint changes are significantly harder to review, test, and benchmark.
2. **Propose Major Changes First:** For non-trivial architectural modifications, new benchmark suites, or breaking API changes, open an issue to discuss design and scope before writing code.
3. **Fork and Branch:** Fork the target repository and create a dedicated feature branch from `main`. Use descriptive branch prefixes (`feat/...`, `fix/...`, `perf/...`, `docs/...`).
4. **Commit & PR Title Standards:** Every commit and pull request title must strictly conform to [Conventional Commits](https://www.conventionalcommits.org/):
   ```text
   <type>(<scope>): <subject>
   ```
   - **Allowed Types:**
     - `feat`: A new feature or capability.
     - `fix`: A bug fix.
     - `perf`: Performance improvements and benchmark speedups.
     - `refactor`: Code changes that neither fix a bug nor add a feature.
     - `docs`: Documentation-only updates.
     - `test`: Adding or correcting tests and benchmark harnesses.
     - `build`: Toolchain, dependency, or compilation updates.
     - `ci`: CI/CD workflows, runners, and automation.
     - `chore`: Maintenance tasks not modifying source or test logic.
     - `style`: Formatting changes that do not affect code semantics.
   - **Scopes:** Use the specific module or project scope (e.g., `feat(vectordb): add HNSW recall@k evaluation pipeline`, `fix(recommender): resolve rating decay in CF model`).
   - **Breaking Changes:** Include `!` before the colon (e.g., `feat(api)!: migrate to typed query responses`) or add a `BREAKING CHANGE:` footer.
5. **Testing and Verification:**
   - Ensure all existing unit tests, integration tests, and benchmarks pass locally.
   - Add new automated tests for any added functionality or bug fixes.
   - Verify code formatting and linter checks pass with clean exit codes.
6. **PR Description & Transparency:**
   - Complete all sections in the pull request template: **Rationale**, **Changes included**, **Test verification**, and **User-facing changes** (breaking changes or critical fixes).
   - Disclose AI-generated assistance in accordance with the transparency checklist.

## Reporting Bugs and Enhancements

- **Bug Reports:** Use the structured Bug Report form under `.github/ISSUE_TEMPLATE`. Include reproducible code snippets, error output, version/commit hash, and select the affected component(s).
- **Enhancement Requests:** Use the Enhancement Request form to detail the problem statement, proposed solution, and affected component(s).
- **Discussions:** For broader architectural questions or benchmark methodology inquiries, join our community discussions.

## Code Review

All submissions are reviewed by the maintainer. Keep pull requests focused on a single change set with concise diffs to facilitate prompt review.
