# Contributing to Fuyu

This short document outlines the standard procedures adopted by all Fuyu
repositories. Please read it before contributing. Every repository may have
additional contributing guidelines with project‑specific information that
build upon these basic guidelines.

**Table of Contents**

- [Code of Conduct](#code-of-conduct)
- [Get Involved](#get-involved)
- [Issues](#issues)
- [Making Changes](#making-changes)
- [Code Conventions](#code-conventions)
- [Pull Requests](#pull-requests)
- [Commits](#commits)

## Code of Conduct

Fuyu has adopted the Contributor Covenant Code of Conduct. Please read the
[Code of Conduct][fuyulang-code-of-conduct] to understand the community rules.

## Get Involved

There are several ways to get involved:

- Start using Fuyu projects!
- Join in on [Fuyu Discussions][fuyulang-discussions]. Ask questions,
  share ideas, and show off the awesome things that you make!
- Look through open [issues](#issues) to contribute fixes and information.

## Issues

Every repository uses [GitHub Issues][github-issues].

### Labels and Issue Types

All repositories use [Issue Types][github-issue-types], which cover general
categories such as Bug and Feature. Repositories may have more specific
[labels][github-labels] to add context to issues.

### Create an Issue

Before creating a new issue, first [search the issues][github-issue-search] to
see if a similar open issue exists. If a similar issue exists, add any
relevant information to the existing issue; otherwise, you can open a new
issue.

**Do not use issues for questions or discussions.** Discussions and support
take place in the [Fuyu Discussions][fuyulang-discussions].

### Fix an Issue

Issues with the following labels are a good place to start:

- `good first issue`: appropriate for new or less‑experienced contributors.
- `help wanted`: appropriate for experienced contributors or those with
  specific expertise.

If you would like to work on an issue, comment on it and a maintainer will
help you get started. After that, submit a [pull request](#pull-requests) with
your changes.

## Making Changes

To submit changes to a Fuyu repository:

1. [Fork the repository][github-fork] and begin making your changes.
2. Follow the appropriate [code conventions](#code-conventions).
3. Test your changes locally.
4. Submit a [pull request](#pull-requests).

## Code Conventions

Fuyu projects attempt to adhere as closely as possible to the language and
tooling conventions used in each project. This helps make the code familiar
for the community.

The best rule is to adopt the style of the project and rely on code
formatters.

## Pull Requests

Take the following steps to submit a pull request:

1. Every pull request must be [linked to an issue][github-pr-link-issue]
   resolved by the pull request.
2. Write an appropriate description of the pull request.
3. Try to follow the [Conventional Commits guidelines](#commits).
4. Submit the pull request.

## Commits

Fuyu uses [Conventional Commits][conventional-commits]. Commit messages
should follow best practices:

- The first line of a commit message must be 50 characters or less.
- Subsequent lines of a commit message must be 72 characters or less.

Fuyu uses the following commit types for its projects:

- `build`: changes to tools, dependencies, and versions.
- `chore`: miscellaneous changes, such as updating `.gitignore`.
- `ci`: changes to continuous integration and continuous delivery.
- `docs`: changes to documentation.
- `feat`: additions, removals, or changes to features.
- `fix`: fixes to defects introduced by `feat` commits.
- `perf`: refactors that improve performance.
- `refactor`: changes that do not affect behaviour.
- `revert`: reverts to previous commits.
- `style`: changes to style or formatting that do not affect behaviour.
- `test`: additions, removals, changes, or fixes to tests.

When contributing, do not worry too much about the exact format of the commit
message. When a pull request is merged into the `main` branch, it is likely
that all commits in the pull request will be squashed, and a maintainer will
provide an appropriate commit message.

Every repository uses [commitlint][commitlint] to enforce consistent rules for
commits, and the configuration is based on the
[default Fuyu .commitlintrc.yml](.commitlintrc.yml).

[commitlint]: https://github.com/conventional-changelog/commitlint
[conventional-commits]: https://www.conventionalcommits.org
[fuyulang-code-of-conduct]: https://github.com/fuyulang/.github/blob/main/CODE_OF_CONDUCT.md
[fuyulang-discussions]: https://github.com/orgs/fuyulang/discussions
[fuyulang-organization]: https://github.com/fuyulang
[github-fork]: https://docs.github.com/en/get-started/quickstart/fork-a-repo
[github-issue-search]: https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments
[github-issue-types]: https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/managing-issue-types-in-an-organization
[github-issues]: https://docs.github.com/en/issues/tracking-your-work-with-issues
[github-labels]: https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels
[github-pr-link-issue]: https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue
