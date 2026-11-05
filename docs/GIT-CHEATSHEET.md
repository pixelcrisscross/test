# Git command cheat sheet

Use these commands in the VS Code terminal. Replace placeholders before running them.

## Check Git and set your identity

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "your-verified-github-email@example.com"
```

Use an email associated with your GitHub account. If you do not want your personal email shown in commits, use the private `noreply` address shown in your GitHub email settings.

## Start with an existing repository

```bash
git clone https://github.com/OWNER/REPOSITORY.git
cd REPOSITORY
git status
```

## Work on a branch

```bash
git switch -c feature/my-change
```

## Save a change

```bash
git status
git add README.md
git commit -m "Add project documentation"
git log --oneline
```

`git add` stages changes. `git commit` records staged changes in the local repository.

## Connect and publish

```bash
git remote -v
git push -u origin feature/my-change
```

After the first push, later pushes on the same branch can usually use `git push`.

## Get updates

```bash
git switch main
git pull
```

## Useful inspection commands

```bash
git status
git diff
git diff --staged
git branch
git log --oneline --graph --all
```

## Common terms

- **Working directory:** your checked-out files.
- **Staging area:** the changes selected for the next commit.
- **Commit:** a recorded snapshot of staged changes.
- **Branch:** a movable line of development.
- **Remote:** a named connection to a repository hosted elsewhere, often GitHub.
- **Push:** send local commits to a remote.
- **Pull:** fetch remote changes and integrate them into the current branch.
- **Pull request:** a GitHub proposal to merge changes from one branch into another.
