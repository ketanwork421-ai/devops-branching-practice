# devops-branching-practice
Git branching and collaboration practice - VERSION A
## Git Branching Workflow

### Branches
- main: Stable production-ready code.
- development: Integration branch for ongoing development.
- feature branches: Used for individual tasks.

### Contribution Workflow
1. Switch to the development branch.
2. Pull the latest changes.
3. Create a feature branch.
4. Make changes to the code.
5. Commit the changes.
6. Push the feature branch to GitHub.
7. Create a Pull Request targeting development.
8. Request a review.
9. Merge after approval.

### Git Commands
- git switch development
- git pull origin development
- git switch -c feature/my-feature
- git add .
- git commit -m "Describe your changes"
- git push

### Pull Request Rules
- Never directly push feature work to main.
- Use feature branches for development.
- Review changes before merging.