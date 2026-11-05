## Mission 2: Write Markdown and make your first commit ✍️

Great work! You created a branch. Now you can make a change without touching `main`.

### Quick lesson: README and Markdown

A `README.md` is the front page of a repository. It introduces the project and usually explains what it does, how to use it, and how to contribute.

Markdown is a lightweight text-formatting language. The `.md` extension is commonly used for Markdown files. GitHub renders Markdown into formatted headings, lists, links, tables, and code blocks.

For this mission, you will create `PROFILE.md`. This is a practice file; it is **not** the special GitHub profile README.

### Activity: create `PROFILE.md`

1. Stay on the `my-first-branch` branch.
2. Select **Add file → Create new file**.
3. Name the file exactly `PROFILE.md` in the repository root.
4. Add your own content using this Markdown structure:

   ```markdown
   # Hi, I'm YOUR NAME 👋

   ## About me
   I am a student and I am learning Git and GitHub.

   ## Interests
   - Open source
   - Web development
   - AI / Data Science

   ## Find me
   - GitHub: https://github.com/YOUR-USERNAME
   ```

5. Replace the placeholders. Do not publish private contact information, passwords, API keys, or tokens.
6. Use the **Preview** tab to see how GitHub renders your Markdown.
7. Click **Commit changes**. Use this commit message: `Add PROFILE.md`.
8. Commit directly to `my-first-branch` (not `main`).

### What is a commit?

A **commit** records a snapshot of staged changes in Git history. Its message should briefly explain what changed. In the GitHub web editor, clicking **Commit changes** creates the commit for you.

**Expected result:** a non-empty `PROFILE.md` file exists at the repository root on `my-first-branch` and begins with a Markdown heading.

The automated checker will verify the file and unlock Mission 3.

### Need help?

- Check the branch selector before creating the file.
- The file name must be `PROFILE.md` (uppercase letters).
- The file must be in the repository root, not inside a folder.
- Make sure the file contains a heading beginning with `# `.
- Commit the change to `my-first-branch`.
