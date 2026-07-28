# ╔═══════════════════════════╗
# ║     GIT CHEAT SHEET       ║
# ╚═══════════════════════════╝

> a quick-reference guide for getting your local code onto github.

### ❯ commiting a new folder

| step | action | command |
|:---|:---|:---|
| **01** | **initialize** (skip if cloned) | `git init` |
| **02** | **connect remote** | `git remote add origin https://github.com/hcg-leo/*` |
| **03** | **set branch** | `git branch -M main` |
| **04** | **stage files** (`.` for all) | `git add .` |
| **05** | **commit** | `git commit -m "<your_message>"` |
| **06** | **push** | `git push -u origin main` |

### ❯ committing a cloned folder

| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git status` |
| **02** | **stage changes** (`.` for all) | `git add .` |
| **03** | **commit changes** | `git commit -m "*"` |
| **04** | **push changes** | `git push` |

