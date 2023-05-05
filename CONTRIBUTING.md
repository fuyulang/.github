# Contributing to Fuyu

Welcome to Fuyu! This short document outlines the standard procedures for all
[Fuyu repositories on GitHub](https://github.com/fuyulang), so please give it
a read before contributing.

Individual repositories may have their own contributing guidelines with project
specific information.

**Table of Contents**

- [Code of Conduct](#code-of-conduct)
- [Get Involved](#get-involved)
- [Issues](#issues)
- [Making Changes](#making-changes)
- [Code Conventions](#code-conventions)
- [Pull Requests](#pull-requests)
- [Commits](#commits)



## Code of Conduct

Fuyu has adopted the _Contributor Covenant Code of Conduct_. Please read the
[full text](https://github.com/fuyulang/.github/blob/main/CODE_OF_CONDUCT.md)
to understand the rules of the Fuyu community before contributing.



## Get Involved

There are several simple ways to get involved in Fuyu:

- Start using Fuyu projects!
- Look through open [issues](#issues) to provide fixes, workarounds, request
  information, and add labels.
- If there is an [issue](#issues) you would like to work on then please submit
  a [pull request](#pull-requests) for it.
- Join in on [Fuyu Discussions](https://github.com/orgs/fuyulang/discussions).
  Ask questions, answer questions, share ideas, share knowledge, and show off
  the awesome things that you make!



## Issues

All issues live on GitHub in the
[issue tracker](https://docs.github.com/en/issues/tracking-your-work-with-issues)
associated with the repository.

### Create an Issue

When creating a new issue, first
[search if an issue already exists](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments).
If a related issue exists, please add any relevant information on the existing
issue, otherwise, you can open a new issue.

**Please do not use issues for questions.** For support, ask in the
[Fuyu Discussions](https://github.com/orgs/fuyulang/discussions).

### Fix an Issue

Issues with the `good first issue` label are a great place to start for
newcomers. The `help wanted` labels are good issues for someone with
knowledge in a specific area to contribute.

We generally do not assign issues to anyone, however, if you would like to fix
an issue then please submit a [pull request](#pull-requests) with your fix.



## Making Changes

To submit changes to a Fuyu repository:

- [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the
  repository and begin making your changes.
- Be sure to follow the appropriate [code conventions](#code-conventions).
- Test your changes locally.
- When you are satisfied with your changes, submit a
  [pull request](#pull-requests).



## Code Conventions

Fuyu uses code formatters wherever possible. The best general rule is to keep
code in the style of the rest of the project.



## Pull Requests

Once you have made changes and are ready to submit a pull request (PR), you
should take the following steps:

- If solving a bug or adding a feature, please submit an issue first that will
  be addressed by the PR.
- Start your PR by filling out the template with all relevant information.
- Enable the
  [checkbox to allow maintainer edits](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
  so the branch can be updated by a maintainer in preparation for a merge.
- When fixing an issue,
  [link your pull request to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
  fixed by your pull request.
- A project maintainer may comment on your pull request to ask for additional
  information or suggest changes.
- All Fuyu projects use [Conventional Commits](#commits). Do not worry so much
  about the commit messages for your pull requests. When a pull request is
  merged, it will be squashed into a single commit and a project maintainer
  will help you come up with the appropriate commit message.
- Be sure to mark conversions as
  [resolved](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request#resolving-conversations)
  when you make changes to the pull request.



## Commits

Fuyu uses [Conventional Commits](https://www.conventionalcommits.org). For all
details, the [full text](https://www.conventionalcommits.org) can be read. In
summary, commits have the following form:

```plaintext
<type>[optional scope]: <description>

[optional body]

[optional footer]
```

The _type_ is one of:

- `build`: changes to the build system
- `chore`: regular maintenance
- `ci`: changes to continuous integration
- `docs`: changes to only documentation
- `feat`: a new feature
- `fix`: a bug fix
- `misc`: anything not covered by a different type, like GitHub templates or
  small README updates
- `perf`: performance improvements
- `refactor`: a code change which neither adds a feature nor fixes a bug
- `revert`: a revert to a previous commit
- `style`: changes not affecting the meaning of the code
- `test`: changes to only testing code

The _scope_ is used to add which parts of the project are changed, such as
`core` or `docs`. The available scopes will be different across

For example, a commit message which _fixes_ a bug in in the _core_ scope may
look like:

```plaintext
fix(core): null dereference leading to crash

A null check was added which prevents a segmentation fault through
dereferencing a null pointer.
```

A body may be included if the short commit description cannot adequately
describe the change.

When contributing do not worry too much about the format of the commit message.
When a pull request is merged into the `main` branch, all commits in the pull
request will be squashed and a maintainer will help by providing an appropriate
commit message.
