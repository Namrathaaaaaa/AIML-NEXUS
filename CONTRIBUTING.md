# Contributing to AIML-NEXUS

Thank you for considering contributing! This guide explains how to fork the repository and create a Pull Request (PR) from your GitHub account

## Fork the repository (web)

1. Open: https://github.com/Namrathaaaaaa/AIML-NEXUS
2. Click the **Fork** button (top-right) and select your account.

After forking, your copy will be at: `https://github.com/<your-username>/AIML-NEXUS`.

## Clone your fork (CLI)

```bash
# replace <your-username> with your GitHub username
git clone https://github.com/<your-username>/AIML-NEXUS.git
cd AIML-NEXUS
```

## Add upstream remote

```bash
git remote add upstream https://github.com/Namrathaaaaaa/AIML-NEXUS.git
git fetch upstream
```

## Create a feature branch

```bash
# use a descriptive branch name
git switch -c feat/my-feature
```

## Make changes and commit

```bash
git add .
git commit -m "Short, meaningful message describing your change"
```

## Keep branch up-to-date (recommended)

```bash
git checkout main
git fetch upstream
git merge upstream/main
git checkout feat/my-feature
git rebase main
```

Resolve conflicts, then `git rebase --continue` if needed.

## Push and open a PR

```bash
git push -u origin feat/my-feature
```

1. On GitHub, open your fork and click "Compare & pull request" or go to the "Pull requests" tab and click "New pull request".
2. Ensure the base repo is `Namrathaaaaaa/AIML-NEXUS` and the base branch is `main` (or as instructed by maintainers).
3. Add a descriptive title and summary. Reference issues if relevant (e.g., "Fixes #12").
4. Submit the PR.

## Quick web-only edits

1. Edit files directly in your fork on GitHub using the pencil icon.
2. Commit to a new branch and click the green banner to open a PR.

## Checklist (suggested)

- [ ] Branch created from an up-to-date `main`.
- [ ] Clear PR title and description.
- [ ] Tests and linters pass locally (if applicable).
- [ ] No secrets in the diff.

## Troubleshooting

- "Permission denied" or authentication errors: check you're pushing to your fork (`origin`). If using SSH, ensure your SSH key is added to GitHub. For HTTPS, use a personal access token if required.
- Merge conflicts: resolve conflicts in the files, `git add` the resolved files, then `git rebase --continue`.
- Accidentally committed to `main`: create a branch from that commit and open a PR. If sensitive data was pushed, contact the maintainers immediately.

If you want the same content added into `README.md` instead, or a shorter web-only guide, tell me and I will update the file accordingly.
