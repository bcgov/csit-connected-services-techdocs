# How to Contribute to `csit-connected-services-techdocs` on Windows

## Purpose

This guide walks you through, step by step, how to:

- install required tools
- configure Git
- clone the repository
- open the project in VS Code
- create a branch
- make changes
- commit using the required format
- push changes
- create a pull request
- assign reviewers

---

## Repository

- URL: https://github.com/bcgov/csit-connected-services-techdocs
- Default branch: `main`

---

# 1. Install Required Tools (Using CMD)

## IMPORTANT

Run Command Prompt as Administrator:

1. Press Start
2. Type `cmd`
3. Right-click **Command Prompt**
4. Click **Run as administrator**

---

## 1.1 Install Git for Windows

```
winget install --id Git.Git -e --source winget
```

---

## 1.2 Install Visual Studio Code

```
winget install --id Microsoft.VisualStudioCode -e --source winget
```

---

## ⚠️ Important: Restart Command Prompt

After installing tools:

- Close Command Prompt
- Open a **new** Command Prompt window

---

## Verify Installations

```
git --version
code --version
```

---

# 2. Configure Git (ONE TIME SETUP)

Use your GitHub email.

```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

# 3. Create a Directory for your Git projects

The directory will be where you check out the git repository.  If you already have one you can skip the creation and just navigate there within the Command Prompt. 

In this example we are creating a **Git** folder within the user's **Documents** folder and then navigating there.


```
mkdir %USERPROFILE%\Documents\Git
cd %USERPROFILE%\Documents\Git
```

---

# 4. Clone the Repository

This step assuems that you have already navigated to your Git project directory. 

```
git clone https://github.com/bcgov/csit-connected-services-techdocs.git
cd csit-connected-services-techdocs
```

---

# 5. Open the Repository in VS Code

This step opens VS Code from the Command Propt and assumes that you have already navigated to the repository directory within your Git project directory.

Alternately, you can search for VS Code (Visual Studio Code) using the windows Start Menu and open it from there.  You will then have to use the VS Code File Menu to open the repository directory.

```
code .
```

---

## Verify

You should see:

- `getting-started/`
- `catalog-info.yaml`
- `README.md`

---

## Trust Workspace

Click **Yes, I trust the authors**

---

# 6. Create a Branch

The document uses the branch `feature/update-getting-started-docs` as an example but you will need to come up with your own unique branch name based on the changes you are planning to make.  
Your branch name should always start with the prefix `feature/`.  
It is a good practice to NOT reuse branch names even after they have been merged and deleted as this can confuse some tools.   

**Remember to update the brach name with the name of your actual branch.**

```
git checkout -b feature/update-getting-started-docs
```

---

# 8. Make Changes

- Edit `.md` files in VS Code
- Save files

Unsaved changes will not be found by Git and will be excluded from the commit. You can turn on Auto-save in VS Code in the File Menu.

---

# 9. Review Changes

```
git status
git diff
```

---

# 10. Commit Changes

You commit message should identify the task under which you are making the change and include a brief description of your changes. 
This step will only commit your changes locally and you will still need to Push the changes to the remote repository.

**Remember to update the brach name with the name of your actual branch.**

```
git add .
git commit -m "API-4555 Update getting started documentation"
```

---

# 11. Push Changes

**Remember to update the brach name with the name of your actual branch.**

```
git push -u origin feature/update-getting-started-docs
```

---

# 12. Create Pull Request

Go to:

https://github.com/bcgov/csit-connected-services-techdocs

Click:

**Compare & pull request**

---

# 13. Assign Reviewers

- Add reviewers on right side

---

# 14. Address Feedback

If your reviewers provide feedback that requires making additional changes you can edit your local files and then add a commit for those changes using the steps below:

```
git add .
git commit -m "API-4555 Address review feedback"
git push
```

---

# 15. Publishing changes to APS Dev Environment

The APS Dev Environment (https://csit-devhub-apps-gov-bc-ca.dev.api.gov.bc.ca/) is configured to load the Connected Services TechDocs from the `dev` branch, so the APS Dev Environment can be updated with your latest changes by pointing the `dev` branch to the same commit as your feature branch.  This can be done as soon as you have pushed your changes to the remote repository.  If you add another commit to your feature branch (as part of the review process), then you will need to repoint the `dev` branch for the APS Dev Environment to reflect those changes.

**Remember to update the brach name with the name of your actual branch.**

```
git push origin feature/update-getting-started-docs:dev --force
```

---

# 16. Common Errors and Fixes

## ❌ Error: `git is not recognized`

**Cause:** Git not installed or CMD not restarted

**Fix:**

- Close CMD
- Open a new CMD window
- Run:

```
git --version
```

---

## ❌ Error: `code is not recognized`

**Cause:** VS Code PATH not loaded

**Fix:**

- Close CMD
- Open new CMD
- Try again:

```
code .
```

If still broken:

- Restart your computer

---

## ❌ Error: `fatal: not a git repository`

**Cause:** Not in repo folder

**Fix:**

```
cd csit-connected-services-techdocs
```

---

## ❌ Error: `permission denied` or authentication failed

**Cause:** Not logged into GitHub

**Fix:**

Run:

```
git push
```

Then:

- Sign in when prompted in browser

---

## ❌ Error: `failed to push` (non-fast-forward)

**Cause:** Remote has newer changes

**Fix:**

```
git pull --rebase origin main
git push
```

---

## ❌ Error: branch already exists

**Fix:**

```
git checkout feature/your-branch-name
```

---

## ❌ Error: uncommitted changes blocking checkout

**Fix (safe):**

```
git stash
```

---

## ❌ Error: accidentally committed wrong files

**Fix (before push):**

```
git reset --soft HEAD~1
```

---

## ❌ Error: pushed wrong commit

**Fix:**

- Ask for help (do not force push unless instructed)

---