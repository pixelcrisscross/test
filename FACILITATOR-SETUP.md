# Facilitator setup — do this before the workshop

This folder is the **template repository source**. Participants must each create a separate repository from it using **Use this template**.

## 1. Create the template repository

1. Sign in to the GitHub account that will own the exercise template (for example, `pixelcrisscross`).
2. Create a new **public, empty** repository named `GDGoC-VTU-GitHub-Bootcamp` with `main` as the default branch. Do not pre-create a README, license, or `.gitignore` on GitHub; the ZIP already contains them.
3. Extract the ZIP and push the contents of this folder to the repository root. Use Git rather than the browser's upload UI so that hidden `.github/` files are included.

   ```bash
   cd GDGoC-VTU-GitHub-Bootcamp
   git init
   git branch -M main
   git add .
   git commit -m "Add interactive GDGoC GitHub bootcamp exercise"
   git remote add origin https://github.com/OWNER/GDGoC-VTU-GitHub-Bootcamp.git
   git push -u origin main
   ```

   Replace `OWNER` with the GitHub username or organization that owns the repository.

4. On the repository page, open **Settings → General → Template repository** and enable **Template repository**.
5. Open **Settings → Actions → General**. Ensure GitHub Actions and the required reusable workflows/actions are permitted by the repository or organization policy.
6. Open the **Actions** tab and enable workflows if GitHub prompts you to do so.

## 2. Test before inviting participants

1. Click **Use this template → Create a new repository** and create a public test repository under a separate test account if possible.
2. Open its **Actions** tab and confirm **Step 0** runs successfully.
3. Confirm that an issue appears with the title `Exercise: GDGoC VTU GitHub Bootcamp — The First Contribution`.
4. Follow all four missions in the test repository, including a test merge.
5. Delete the test repository after testing if it is no longer needed.

Do not use the template itself as a learner repository. The start workflow intentionally skips the template repository.

## 3. Participant link

After the template repository exists, participants can create their own copy from:

`https://github.com/OWNER/GDGoC-VTU-GitHub-Bootcamp/generate`

Replace `OWNER` with the actual owner. Share this link as a QR code. Ask participants to choose **Public** and a distinct repository name.

## 4. What runs automatically

| Workflow | Trigger | Result |
|---|---|---|
| Step 0 | Push to `main` or manual `workflow_dispatch` in a repository created from the template | Creates the exercise issue and posts Mission 1 |
| Step 1 | Push to `my-first-branch` | Posts Mission 2 |
| Step 2 | Push of `PROFILE.md` to `my-first-branch` | Validates the file and posts Mission 3 |
| Step 3 | PR to `main` from `my-first-branch` | Checks PR title and description, then posts Mission 4 |
| Step 4 | PR closed | Completes the exercise if merged; otherwise re-enables the PR check |

The workflow files request only the permissions needed for their operations. Organization-level policies can still restrict Actions or token permissions.

## 5. Troubleshooting

- **No issue appears:** open **Actions → Step 0** and inspect the run log. Confirm that Actions are enabled and the new repository was created from the template. If the automatic run did not occur and no exercise issue exists yet, use **Run workflow** once as a manual fallback. Do not manually run it if the exercise issue already exists, or you may create a duplicate.
- **No mission unlocks:** check the relevant workflow run and make sure the branch/file/title matches exactly.
- **Actions disabled:** in the learner's repository, open the Actions tab and enable workflows. For this reason, test the template from a clean account before the workshop.
- **Toolkit or action failure:** inspect the failed step in the run log. Re-run only after fixing the underlying issue.
- **PR check does not run:** confirm the PR targets `main` and comes from `my-first-branch` in the participant's own exercise repository.

## 6. Safety and maintenance

- Keep this exercise repository public if you want participants to use it without private-repository Actions usage.
- Never ask participants to add secrets, tokens, passwords, or private information to their profile file.
- Review third-party Actions and reusable workflows before running them. The workflows in this exercise use GitHub Skills' public exercise toolkit and the `GrantBirki/comment` action to post Markdown lessons to the exercise issue.
- Re-test after changing workflow names, branch names, issue titles, or toolkit versions. These values must stay in sync across files.
- GitHub UI labels can change; use the equivalent current control if the interface changes.
