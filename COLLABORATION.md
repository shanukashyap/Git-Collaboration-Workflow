
# Git Collaboration Workflow Evidence

## Project

Git Collaboration Workflow

## Developer A

Developer A created the initial GitHub repository and created the initial version of `app.py`.

Initial application:

```python
print("Welcome to the Git Collaboration Project")

print("This is the initial version of the application.")
```

The initial version was committed and pushed to the `main` branch.

## Developer B

Developer B cloned the remote repository and created a separate feature branch:

```text
add-project-status
```

Developer B then implemented the project status feature.

The feature added to `app.py` was:

```python
print("Project Status: Active")
```

## Branch Workflow

The development workflow was:

```text
main
  |
  | Initial project
  |
  +---- add-project-status
             |
             | Add project status feature
             |
             | Commit
             |
             | Push
             |
             v
       Pull Request
             |
             | Code Review
             |
             | Approval
             |
             v
           main
```

## Git Commands Used

### Developer A

```bash
git init
git add .
git commit -m "Create initial project"
git remote add origin <repository-url>
git branch -M main
git push -u origin main
```

### Developer B

```bash
git clone <repository-url>
git switch -c add-project-status
git add .
git commit -m "Add project status feature"
git push -u origin add-project-status
```

### Fetch and Pull

```bash
git fetch origin
git pull origin main
```

`git fetch` was used to retrieve information about changes from the remote repository.

`git pull` was used to retrieve and integrate the latest changes into the local branch.

## Pull Request

Developer B created a Pull Request from:

```text
add-project-status
```

to:

```text
main
```

Pull Request URL:

```text
https://github.com/shanukashyap/Git-Collaboration-Workflow/pull/1
```

## Code Review

The changes in the Pull Request were reviewed before merging.

The review checked that the new project status feature was correctly added to `app.py`.

## Merge

After the code review, the Pull Request was merged into the `main` branch.

After the merge, the local `main` branch was updated using:

```bash
git switch main
git fetch origin
git pull origin main
```

## Final Result

The final `main` branch contains the project status feature:

```python
print("Project Status: Active")
```

## Evidence

The GitHub repository contains:

* `main` branch
* `add-project-status` feature branch
* Feature commit
* Pull Request
* Code review
* Pull Request merge
* Updated `main` branch

Repository URL:

```text
 ACTUAL GITHUB REPOSITORY URL HERE

https://github.com/shanukashyap/Git-Collaboration-Workflow
```

Pull Request URL:

```text
 GITHUB PULL REQUEST URL HERE
https://github.com/shanukashyap/Git-Collaboration-Workflow/pull/1
```
