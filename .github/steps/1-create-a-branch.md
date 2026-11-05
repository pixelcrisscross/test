## Mission 1: Create your first branch 🌱

Welcome to the **GDGoC VTU GitHub Bootcamp**!

### First, understand what you are working with

For a fuller glossary, open `docs/BOOTCAMP-CONCEPTS.md` in the **Code** tab.

- A **repository** is the project space that stores files and their Git history.
- A **codebase** is the source code that implements a software project. A repository can also store documentation, tests, images, and configuration.
- A **branch** is an independent line of development. It lets you work on a change without editing the default `main` branch directly.

### Activity: create a branch

1. Open the **Code** tab of this repository.
2. Open the branch selector. It should currently show `main`.
3. In the branch search box, type exactly `my-first-branch`.
4. Choose **Create branch: my-first-branch from main**.
5. Confirm that the branch selector now shows `my-first-branch`.

**Expected result:** this repository now has a branch named `my-first-branch`.

> You can do this in the GitHub website. You do not need a local terminal for this mission.

### Optional: do the same with Git

```bash
git switch -c my-first-branch
```

When the branch is pushed to GitHub, the automated checker will detect it and unlock Mission 2 in this issue.

### Need help?

- Make sure the spelling is exactly `my-first-branch`.
- Create it from `main`.
- If nothing happens, open the **Actions** tab and check whether the **Step 1** workflow is enabled and whether the run succeeded.
