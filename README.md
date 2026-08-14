# ╔═══════════════════════════╗
# ║       LEARNING GIT        ║
# ╚═══════════════════════════╝

> a quick-reference for git commands.

## table of contents
* **[Commit](#commit)**
  * [Committing a cloned folder](#cloned-folder)
  * [Committing a new folder](#new-folder)
  * [Reverting a commit](#reverting)
* **[Branches](#branches)**
  * [Creating branches](#creating-branches)
  * [Want to keep code](#keep-code)

---

# commit

### <a id="cloned-folder"></a>❯ committing a cloned folder

| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git pull` |
| **02** | **status check** | `git status` |
| **03** | **stage changes** (`.` for all) | `git add .` |
| **04** | **commit changes** | `git commit -m "*"` |
| **05** | **push changes** | `git push` |

### <a id="new-folder"></a>❯ committing a new folder

| step | action | command |
|:---|:---|:---|
| **01** | **initialize** (skip if cloned) | `git init` |
| **02** | **connect remote** | `git remote add origin https://github.com/hcg-leo/*` |
| **03** | **set branch** | `git branch -M main` |
| **04** | **stage files** (`.` for all) | `git add .` |
| **05** | **commit** | `git commit -m "*"` |
| **06** | **push** | `git push -u origin main` |

### <a id="reverting"></a>❯ reverting a commit

| step | action | command |
|:---|:---|:---|
| **01** | **commit check** | `git log --oneline` |
| **02** | **checkout** (`.` for all) | `git checkout <your-commit-hash> .` |
| **03** | **commit changes** | `git commit -m "Rolling back to older state from commit <your-commit-hash>"` |
| **04** | **push changes** | `git push` |

# branches

### <a id="creating-branches"></a>❯ creating branches
| step | action | command |
|:---|:---|:---|
| **01** | **status check** | `git status` |
| **--** | **if you don't want to commit** | `git stash` |
| **02** | **create & switch branch** | `git switch -c <*>` |
| **03** | **stage changes** (`.` for all) | `git add .` |
| **04** | **commit changes** | `git commit -m "*"` |

### <a id="keep-code"></a>❯ want to keep code
| step | action | command |
|:---|:---|:---|
| **01** | **switch to main** | `git switch main` |
| **02** | **merge branch** | `git merge <*>` |
| **03** | **delete old branch** | `git branch -d <*>` |
