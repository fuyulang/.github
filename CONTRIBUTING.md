# Contributing to Fuyu

Welcome to Fuyu! This short document outlines the standard procedures for all
[Fuyu repositories on GitHub][fuyulang-github], so please give it a read before
contributing.

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
[full text][code-of-conduct] to understand the rules of the Fuyu community
before contributing.



## Get Involved

There are several simple ways to get involved in Fuyu:

- Start using Fuyu projects!
- Look through open [issues](#issues) to provide fixes, workarounds, request
  information, and add labels.
- If there is an issue you would like to work on then please comment on the
  issue and a maintainer will help you get started.
- Submit a [pull request](#pull-requests) to address an issue after a
  maintainer helps you get started.
- Join in on [Fuyu Discussions][fuyulang-discussions]. Ask questions, answer
  questions, share ideas, share knowledge, and show off the awesome things that
  you make!



## Issues

All issues live on GitHub in the [issue tracker][github-issues] associated with
the repository.

### Create an Issue

Before creating a new issue, first [search the issues][github-search-issues] to
see if a similar one already exists. If a similar issue exists, please add any
relevant information on the existing issue, otherwise, you can open a new
issue.

**Please do not use issues for questions or discussions.** Discussions and
support take place in the [Fuyu Discussions][fuyulang-discussions].

### Fix an Issue

Issues with the `Good first issue` label are a great place to start for
newcomers. Issues with a `Help wanted` label are good issues for more
experienced contributors or those with domain specific knowledge.

We generally do not assign issues to anyone, however, if you would like address
an issue then comment on it and a maintainer will help you get started. After
that, please submit a [pull request](#pull-requests) with your changes.

### Labels

The table below shows the label types that can be used in the issue tracker.
Not all colors in the palette are used, but enough colors were created to
accomodate new categories.

| Color                     | Hex       | Category      |
|---------------------------|-----------|---------------|
| ![red][red]        Red    | `#f5c2b1` | Problem       |
| ![orange][orange]  Orange | `#fdd4aa` | Flags         |
| ![yellow][yellow]  Yellow | `#fbeaae` | -             |
| ![green][green]    Green  | `#bde9be` | -             |
| ![cyan][cyan]      Cyan   | `#a0e0d9` | -             |
| ![blue][blue]      Blue   | `#b8d9f0` | Type          |
| ![purple][purple]  Purple | `#cec9f3` | Area          |
| ![pink][pink]      Pink   | `#eec8f1` | Participation |
| ![white][white]    White  | `#ffffff` | Active        |
| ![gray][gray]      Gray   | `#cccccc` | Inactive      |

The issue categories are intentionally kept broad and using highly specific
labels are avoided. The categories are:

- **Problem**: Bugs, defects, errors, faults, and failures.
- **Flags**: Additional important information (e.g., difficulty, priority).
- **Type**: A change to be made (e.g., feature, documentation, refactor).
- **Area**: A repository specific category for project components.
- **Participation**: How the community can get involved.
- **Active**: State of tasks that are in progress or planned.
- **Inactive**: State of tasks that are not planned.



## Making Changes

To submit changes to a Fuyu repository:

- [Fork][github-fork] the repository and begin making your changes.
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
- Enable the [checkbox to allow maintainer edits][github-pull-request-edits] so
  the branch can be updated by a maintainer in preparation for a merge.
- When fixing an issue, [link your pull request to an issue][github-link-issue]
  fixed by your pull request.
- A project maintainer may comment on your pull request to ask for additional
  information or suggest changes.
- All Fuyu projects use [Conventional Commits](#commits). Do not worry so much
  about the commit messages for your pull requests. When a pull request is
  merged, it will be squashed into a single commit and a project maintainer
  will help you come up with the appropriate commit message.
- Be sure to mark conversions as [resolved][github-resolving-conversations]
  when you make changes to the pull request.



## Commits

Fuyu uses [Conventional Commits][conventional-commits]. For all details please
refer to the [full text][conventional-commits]. In summary, commits have the
following form:

```plaintext
<type>[scope]: <description>

[body]

[footer]
```

> [!IMPORTANT]
> To ensure readability of commits:
>
> - Keep `<type>[scope]: <description>` to 52 characters or less.
> - The `[body]` and `[footer]` are optional and the lines of each should be
>   kept to 72 characters or less.

Fuyu uses the following types for its projects:

- `build`: a change to build processes or project dependencies.
- `change`: a change to an existing feature.
- `chore`: a maintenance activity that is not related to any specific feature.
- `ci`: a change to continuous integration and continuous delivery.
- `deprecate`: a change that deprecates but does not remove functionality.
- `docs`: a change to documentation.
- `feat`: a change that implements a new feature.
- `fix`: a change that fixes a defect.
- `perf`: a performance improvement or optimization.
- `refactor`: a change that does not affect behavior.
- `remove`: a change that removes a feature.
- `revert`: a change that reverts to a previous commit.
- `security`: a change that improves security.
- `style`: a change that does not modify the implementation.
- `test`: a change to testing or reporting.

The scope is used to add which parts of the project are changed, such as
`lexer` or `gc`. The available scopes will be different across different
projects.

For example, a commit message which fixes a bug in in the `gc` scope may
look like:

```plaintext
fix(core): null dereference leading to crash

A null check was added which prevents a segmentation fault through
dereferencing a null pointer.

Resolves: #123
```

A body may be included if the short commit description cannot adequately
describe the change.

When contributing do not worry too much about the format of the commit message.
When a pull request is merged into the `main` branch, all commits in the pull
request will be squashed and a maintainer will help by providing an appropriate
commit message.



[fuyulang-github]: https://github.com/fuyulang
[code-of-conduct]: https://github.com/fuyulang/.github/blob/main/CODE_OF_CONDUCT.md
[fuyulang-discussions]: https://github.com/orgs/fuyulang/discussions
[github-issues]: https://docs.github.com/en/issues/tracking-your-work-with-issues
[github-search-issues]: https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments
[github-fork]: https://docs.github.com/en/get-started/quickstart/fork-a-repo
[github-pull-request-edits]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork
[github-link-issue]: https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue
[github-resolving-conversations]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request#resolving-conversations
[conventional-commits]: https://www.conventionalcommits.org

[red]:    https://dummyimage.com/12x12/f5c2b1.png?text=+
[orange]: https://dummyimage.com/12x12/fdd4aa.png?text=+
[yellow]: https://dummyimage.com/12x12/fbeaae.png?text=+
[green]:  https://dummyimage.com/12x12/bde9be.png?text=+
[cyan]:   https://dummyimage.com/12x12/a0e0d9.png?text=+
[blue]:   https://dummyimage.com/12x12/b8d9f0.png?text=+
[purple]: https://dummyimage.com/12x12/cec9f3.png?text=+
[pink]:   https://dummyimage.com/12x12/eec8f1.png?text=+
[white]:  https://dummyimage.com/12x12/ffffff.png?text=+
[gray]:   https://dummyimage.com/12x12/cccccc.png?text=+
