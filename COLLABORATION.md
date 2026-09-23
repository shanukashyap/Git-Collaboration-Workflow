# Git Collaboration Workflow

## Project Name

Git Collaboration Workflow

## Repository

**GitHub Repository:**
PASTE YOUR ACTUAL PUBLIC GITHUB REPOSITORY URL HERE

## Pull Request

**Pull Request:**
PASTE YOUR ACTUAL PULL REQUEST URL HERE

---

# 1. Project Objective

This project demonstrates a two-developer Git and GitHub collaboration workflow.

The workflow includes:

* Remote repository
* Clone
* Branch creation
* Feature development
* Commit
* Push
* Fetch
* Pull
* Pull Request
* Code review
* Merge into `main`

Since this project was completed individually, two branches were used to simulate two developers.

---

# 2. Developer Roles

## Developer A

Developer A was responsible for:

* Creating the GitHub repository
* Creating the initial application
* Creating the initial commit
* Creating the `main` branch
* Connecting the local repository to GitHub
* Pushing the initial project to `main`

## Developer B

Developer B was responsible for:

* Cloning the repository
* Creating the `add-project-status` branch
* Implementing the project status feature
* Testing the feature
* Committing the changes
* Pushing the feature branch
* Creating the Pull Request
* Participating in the code review process

---

# 3. Branches Used

The project used the following branches:

```text
main
add-project-status
```

### Main Branch

The `main` branch contains the initial project and the final merged version.

### Feature Branch

The `add-project-status` branch was used by Developer B to implement the project status feature without directly modifying `main`.

---

# 4. Initial Version

Developer A created the initial version of `app.py`.

The initial application contained:

```python
print("Welcome to the Git Collaboration Project")

print("This is the initial version of the application.")
```

The initial version was committed and pushed to the `main` branch.

---

# 5. Developer B Feature

Developer B cloned the repository and created:

```text
add-project-status
```

The feature branch added a project status display function.

The implemented feature is:

```python
def display_project_status():
    """Display the current status of the project."""
    status = "Active"
    print(f"Project Status: {status}")


display_project_status()
```

The feature displays:

```text
Project Status: Active
```

This demonstrates that Developer B made a visible code contribution through a separate feature branch.

---

# 6. Git Workflow

The complete workflow was:

```text
Developer A
     |
     v
Create GitHub Repository
     |
     v
Create Initial Project
     |
     v
Commit
     |
     v
Push to main
     |
     v
GitHub Remote Repository
     |
     v
Developer B
     |
     v
Clone Repository
     |
     v
Create add-project-status Branch
     |
     v
Implement Feature
     |
     v
Commit
     |
     v
Push Feature Branch
     |
     v
Pull Request
     |
     v
Code Review
     |
     v
Merge into main
     |
     v
Updated main Branch
```

---

# 7. Git Commands Used

## Developer A — Initial Repository

```bash
git init
git add .
git commit -m "Create initial project"
git remote add origin <repository-url>
git branch -M main
git push -u origin main
```

## Developer B — Clone

```bash
git clone <https://github.com/shanukashyap/Git-Collaboration-Workflow>
cd Git-Collaboration-Workflow
```

## Create Feature Branch

```bash
git switch -c add-project-status
```

## Check Branch

```bash
git branch
```

Expected:

```text
* add-project-status
  main
```

## Check Changes

```bash
git status
git diff
```

## Commit Feature

```bash
git add app.py
git commit -m "Add project status display function"
```

## Push Feature Branch

```bash
git push -u origin add-project-status
```

---

# 8. Fetch

The following command was used to retrieve information from the remote repository:

```bash
git fetch origin
```

`git fetch` downloads information about remote changes without automatically merging those changes into the current branch.

---

# 9. Pull

After the Pull Request was merged, the local `main` branch was updated using:

```bash
git switch main
git pull origin main
```

`git pull` retrieves the latest changes from the remote repository and integrates them into the current branch.

---

# 10. Pull Request

Developer B created a Pull Request from:

```text
add-project-status
```

to:

```text
main
```

## Pull Request URL

PASTE YOUR ACTUAL GITHUB PULL REQUEST URL HERE

The Pull Request was used to propose the feature for review before it was merged into the `main` branch.

---

# 11. Code Review

The Pull Request was reviewed before merging.

The review checked:

* Whether the new function was correctly implemented
* Whether the project status was displayed correctly
* Whether the change was limited to the intended feature
* Whether the application continued to run successfully

The feature was then approved for merging.

---

# 12. Merge

After the code review, the Pull Request was merged into:

```text
main
```

The final branch structure was:

```text
main
 |
 +-- Initial project
 |
 +-- Merge Pull Request
       |
       +-- Project status display feature
```

---

# 13. Final Feature

After the merge, the final application displays:

```text
Welcome to the Git Collaboration Project
This is the initial version of the application.
Project Status: Active
```

The final `main` branch contains the feature originally developed in the `add-project-status` branch.

---

# 14. Repository Evidence

## Public Repository


https://github.com/shanukashyap/Git-Collaboration-Workflow

## Pull Request

https://github.com/shanukashyap/Git-Collaboration-Workflow/pull/1

## Branches

```text
main
add-project-status
```

## Feature Commit

```text
Add project status display function
```

## Merge Result

The `add-project-status` feature branch was reviewed through a Pull Request and merged into `main`.

---

# 15. Learning Outcomes

This project demonstrates practical Git and GitHub collaboration concepts:

* Local Git repository
* Remote GitHub repository
* `git clone`
* `git fetch`
* `git pull`
* `git push`
* Branch creation
* Feature development
* Commits
* Pull Requests
* Code review
* Merge
* Two-developer workflow simulation

---

# 16. Conclusion

This project demonstrates how multiple developers can collaborate safely using Git and GitHub.

Developer A created the initial project on `main`.

Developer B worked independently on the `add-project-status` feature branch, committed and pushed the feature, and created a Pull Request.

The changes were reviewed and then merged into `main`.

This workflow prevents developers from directly making unreviewed changes to the main branch and provides a structured process for collaboration.
