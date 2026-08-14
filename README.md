# ╔═══════════════════════════╗
# ║     GIT CHEAT SHEET       ║
# ╚═══════════════════════════╝

> a quick-reference guide for getting your local code onto github.

# commit
### ❯ committing a cloned folder

| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git pull` |
| **02** | **status check** | `git status` |
| **03** | **stage changes** (`.` for all) | `git add .` |
| **04** | **commit changes** | `git commit -m "*"` |
| **05** | **push changes** | `git push` |
### ❯ commiting a new folder

| step | action | command |
|:---|:---|:---|
| **01** | **initialize** (skip if cloned) | `git init` |
| **02** | **connect remote** | `git remote add origin https://github.com/hcg-leo/*` |
| **03** | **set branch** | `git branch -M main` |
| **04** | **stage files** (`.` for all) | `git add .` |
| **05** | **commit** | `git commit -m "*"` |
| **06** | **push** | `git push -u origin main` |

### ❯ reverting a commit

| step | action | command |
|:---|:---|:---|
| **01** | **commit check** | `git log --oneline` |
| **02** | **checkout** (`.` for all) | `git checkout <your-commit-hash> .` |
| **03** | **commit changes** | `git commit -m "Rolling back to older state from commit <your-commit-hash>"` |
| **04** | **push changes** | `git push` |

# branches
### ❯ creating branches
| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git status` |    | **if you dont want to commit** | `git stash` |
| **02** | **checkout** (`.` for all) | `git switch -c <*>` |
| **03** | **commit changes** | `git add .` |
| **04** | **push changes** | `git commit -m "*"` |

### ❯ want to keep code
| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git switch main` |
| **02** | **checkout** (`.` for all) | `git merge <*>` |
| **03** | **commit changes** | `git branch -d <*>` |

### ❯ want to delete code
| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git switch main` |
| **02** | **checkout** (`.` for all) | `git branch -D <*>` |
