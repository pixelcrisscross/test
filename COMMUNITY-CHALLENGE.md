# Bonus mission: contribute to the GDGoC community

You have completed the guided exercise in your personal copy. Now make a contribution to a shared project.

**Upstream repository:** [pixelcrisscross/Welcome-to-the-Community](https://github.com/pixelcrisscross/Welcome-to-the-Community)

> The repository owner should prepare the upstream repository with a README and contribution instructions before the workshop. Check the repository page for the latest instructions.

## Your task

1. Open the upstream repository and click **Fork**.
2. Clone your own fork, not the upstream repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/Welcome-to-the-Community.git
   cd Welcome-to-the-Community
   ```

3. Create a branch:

   ```bash
   git switch -c add-my-community-profile
   ```

4. Create a file named `contributors/YOUR-GITHUB-USERNAME.md`.
5. Add a short introduction using Markdown. Example:

   ```markdown
   # Your Name

   - GitHub: https://github.com/YOUR-GITHUB-USERNAME
   - Interests: Open source, AI, web development
   - What I want to learn: Building with a community
   ```

6. Stage, commit, and push:

   ```bash
   git add contributors/YOUR-GITHUB-USERNAME.md
   git commit -m "Add my community profile"
   git push -u origin add-my-community-profile
   ```

7. Open a pull request from your fork to the upstream repository's `main` branch. Explain what you added.
8. Respond politely to review feedback. The maintainers decide whether and when to merge contributions.

## Good open-source habits

- Read the upstream README and `CONTRIBUTING.md` before making changes.
- Keep your change small and relevant.
- Never include secrets or personal contact details.
- A submitted pull request is a proposal, not a guarantee of acceptance or organization membership.
