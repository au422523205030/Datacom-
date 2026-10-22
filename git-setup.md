# Git setup and command guide

## Verify Git is installed

```bash
git --version
```

## Set your identity (use your own name and GitHub email)

```bash
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR GITHUB EMAIL"
git config --global --list
```

## Clone an empty repository

On GitHub, create a repository without a README or other initial files. Copy its HTTPS URL from **Quick setup**, then run:

```bash
git clone YOUR_REPOSITORY_HTTPS_URL
cd datacom-introduction-to-cloud
```

## Save and upload project changes

```bash
git status
git add .
git commit -m "Add first GitHub Actions workflow"
git push -u origin main
```

## Key terms

- **Git:** version-control software installed on your computer.
- **GitHub repository:** the online project space.
- **Clone:** copy the online repository to your computer.
- **Commit:** save a snapshot of changes in Git history.
- **Push:** upload local commits to GitHub.
- **Workflow:** a YAML file that automates steps on GitHub-hosted machines.
- **Variable:** a named value that can be reused in a workflow.
- **Secret:** protected storage for sensitive values such as tokens or passwords.
