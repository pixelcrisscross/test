# Bootcamp concepts: the GitHub project anatomy

## Codebase versus repository

A **codebase** is the source code that implements a software project. A **repository** is the version-controlled project space that holds files and their history. A repository may include a codebase, but it can also contain documentation, datasets, tests, images, configuration, and workflows. A documentation-only repository may have no application source code at all.

## Git versus GitHub

- **Git** is a distributed version-control system. It records snapshots as commits and supports branching and merging.
- **GitHub** hosts Git repositories and adds collaboration features such as pull requests, issues, discussions, projects, releases, and Actions.

## README.md

A repository README is its front page. It should answer: What is this project? Why does it exist? How do I install or use it? How can I contribute? GitHub displays a README from the repository's `.github`, root, or `docs` directory (using its documented precedence).

A **profile README** is different: create a public repository whose name exactly matches your GitHub username and put a non-empty `README.md` in the root. GitHub can display that README at the top of your profile. The `PROFILE.md` file in this exercise is only a practice file; it is not a profile README.

## Markdown (.md)

Markdown is a lightweight markup syntax for readable plain text. `.md` is a commonly used filename extension. GitHub renders Markdown in README files, issues, pull requests, discussions, and other places. It supports headings, emphasis, lists, links, images, tables, task lists, blockquotes, and code blocks. See `docs/MARKDOWN-QUICKSTART.md` in this repository.

## Common repository files

| Path | Purpose |
|---|---|
| `README.md` | Project overview, setup, usage, contribution links |
| `LICENSE` | Permissions and conditions for reusing the project |
| `.gitignore` | Patterns for files Git should ignore |
| `CONTRIBUTING.md` | Contribution process and coding expectations |
| `CODE_OF_CONDUCT.md` | Community behaviour expectations (when a project adopts one) |
| `src/` | Common location for source code |
| `tests/` | Common location for automated tests |
| `docs/` | Project documentation |
| `.github/` | GitHub-specific configuration and templates |
| `.github/workflows/` | GitHub Actions workflow definitions |

## The Git change lifecycle

1. Edit files in the **working directory**.
2. Select changes with `git add` for the **staging area**.
3. Record a snapshot with `git commit`.
4. Publish commits with `git push` to a **remote** such as GitHub.
5. Open a **pull request** to propose changes to another branch.
6. Review the diff, discuss it, and **merge** when accepted.

## Collaboration vocabulary

- **Issue:** a trackable task, bug report, or question.
- **Pull request:** a proposal to merge changes from a source branch into a base branch.
- **Review:** feedback on a proposed change.
- **Merge conflict:** a situation where Git cannot automatically reconcile competing changes.
- **GitHub Actions:** event-driven automation configured in YAML workflow files.
- **Release:** a packaged or announced version of a project, often associated with a Git tag.
- **Fork:** your GitHub-hosted copy of someone else's repository.
- **Clone:** a local copy of a repository with its Git history.

## Further reading

- https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories
- https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
- https://docs.github.com/en/get-started/writing-on-github
- https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests
