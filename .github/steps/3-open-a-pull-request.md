## Mission 3: Open your first pull request 🔀

You have a branch and a commit. Now it is time to propose your change to the project.

### What is a pull request?

A **pull request (PR)** is a proposal to merge changes from one branch into another. It gives collaborators a place to inspect the diff, discuss the change, request improvements, and approve the work.

### Activity: open a pull request

1. Open the **Pull requests** tab.
2. Click **New pull request** (or **Compare & pull request** if GitHub shows that shortcut).
3. Set the branches carefully:
   - **base:** `main`
   - **compare:** `my-first-branch`
4. Review the **Files changed** tab. Confirm that your PR adds `PROFILE.md` and does not unexpectedly change other files.
5. Use this exact title: `Add my first profile`.
6. Add a short description explaining what you changed. For example:

   ```text
   ## What changed
   - Added my PROFILE.md file.
   - Practised Markdown headings and lists.

   ## Why
   This is my first contribution in the GitHub bootcamp exercise.
   ```

7. Click **Create pull request**.

### Automated review

GitHub Actions checks that:

- Your PR comes from `my-first-branch`.
- Its title contains `Add my first profile`.
- Its description is not empty.

If a check fails, read the comment on your PR, edit the title or description, and try again. The workflow listens for PR edits.

**Expected result:** the PR checks pass and this issue receives Mission 4.

### Need help?

- Base is the branch receiving the changes: `main`.
- Compare is the branch containing your work: `my-first-branch`.
- A pull request is not the same as a commit. A commit records a change; a PR proposes integrating commits into another branch.
