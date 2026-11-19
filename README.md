# DevOps Branching Practice

A hands-on project to learn Git, GitHub collaboration, branching strategies, Pull Requests, merge conflict resolution, and basic CI/CD using GitHub Actions.

## 1. Branch Structure

- **main:** Stable, production-ready code.
- **development:** Integration branch for ongoing development.
- **feature branches:** Used for individual tasks and new features.

## 2. Contribution Workflow

1. Switch to the development branch.
2. Pull the latest changes.
3. Create a new feature branch.
4. Make changes to the code.
5. Stage and commit the changes.
6. Push the feature branch to GitHub.
7. Create a Pull Request targeting development.
8. Request a code review.
9. Merge the PR after approval.

## 3. Important Git Commands

```bash
# Switch to development
git switch development

# Get latest changes
git pull origin development

# Create a feature branch
git switch -c feature/my-feature

# Stage changes
git add .

# Commit changes
git commit -m "Describe your changes"

# Push feature branch
git push -u origin feature/my-feature
```

## 4. Pull Request Rules

- Never directly push feature work to main.
- Use feature branches for development.
- Create Pull Requests targeting development.
- Review changes before merging.
- Merge after approval.

## 5. Merge Conflict Resolution

A merge conflict occurs when Git cannot automatically combine changes made to the same part of a file.

Practice performed:

1. Created two feature branches: `feature/conflict-a` and `feature/conflict-b`.
2. Modified the same line in README.md with different content.
3. Merged the branches and generated a merge conflict.
4. Identified the conflicting changes.
5. Resolved the conflict by combining both versions.
6. Committed and pushed the resolved changes.

## 6. .gitignore

The `.gitignore` file specifies files and folders that Git should not track.

Examples:

- `.env`
- `node_modules/`
- `*.log`
- `__pycache__/`
- `*.pyc`

## 7. GitHub Actions – Basic CI

A basic CI workflow was created at:

`.github/workflows/ci.yml`

The workflow runs automatically when:

- Code is pushed to the development branch.
- A Pull Request targets the development branch.

The workflow performs these steps:

1. Checks out the repository.
2. Displays a success message.
3. Lists repository files.

The workflow was executed successfully using GitHub Actions.

## 8. Learning Outcomes

- Git branching and branch management.
- Git commits and pushing changes.
- Pull Request creation and merging.
- Code review concepts.
- Merge conflict identification and resolution.
- GitHub Issues, Labels and Milestones.
- .gitignore configuration.
- GitHub Actions and basic Continuous Integration.
- Introduction to CI/CD concepts.
