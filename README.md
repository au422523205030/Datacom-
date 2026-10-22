# Datacom – Introduction to Cloud: GitHub Actions Starter Project

This beginner project demonstrates Git, GitHub repositories, workflow variables, and a first GitHub Actions workflow.

## What this project does

Whenever you push to the `main` branch (or manually start the workflow), GitHub Actions runs a small job that prints a greeting and the project name using variables.

## Files

- `.github/workflows/first-workflow.yml` — the automated workflow.
- `docs/git-setup.md` — setup and Git command guide.

## Setup

1. Create an **empty** GitHub repository named `datacom-introduction-to-cloud` (do not add a README, licence, or `.gitignore` while creating it, because the assignment asks you to clone an empty repository).
2. Install Git: https://git-scm.com/install/
3. Open Git Bash (Windows) or Terminal (macOS/Linux), then configure your Git identity:

   ```bash
   git config --global user.name "YOUR NAME"
   git config --global user.email "YOUR GITHUB EMAIL"
   ```

4. Copy the HTTPS clone URL from the empty repository's **Quick setup** section and run:

   ```bash
   git clone YOUR_REPOSITORY_HTTPS_URL
   cd datacom-introduction-to-cloud
   ```

5. Copy the files in this starter project into the cloned repository folder, keeping the `.github/workflows/` directory structure.
6. Commit and push:

   ```bash
   git add .
   git commit -m "Add first GitHub Actions workflow"
   git branch -M main
   git push -u origin main
   ```

7. Open your repository on GitHub, select **Actions**, and open `First GitHub Actions Workflow`. Confirm that the run finishes successfully.
8. Share your repository URL with the Datacom team using the Teams channel specified in your instructions.

## Variables explained

- `PROJECT_NAME` and `GREETING` are non-sensitive workflow environment variables declared under `env` in the workflow file.
- `${{ env.PROJECT_NAME }}` is GitHub Actions expression syntax for reading a workflow environment variable.
- Never store passwords, tokens, or other sensitive information in ordinary variables. Use GitHub Actions **Secrets** for sensitive values.

## Important

This is a starter project you can upload to your own GitHub repository. It does not create or push to your GitHub account automatically. Replace placeholders in the commands with your own details, and do not share your password or access token.
