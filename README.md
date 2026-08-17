# ╔═══════════════════════════╗
# ║       LEARNING GIT        ║
# ╚═══════════════════════════╝

> a quick-reference for git commands.

## table of contents
* **[Commit](#commit)**
  * [committing a cloned folder](#cloned-folder)
  * [committing a new folder](#new-folder)
  * [reverting a commit](#reverting)
* **[branches](#branches)**
  * [creating branches](#creating-branches)
  * [merge code into main branch](#keep-branch)
  * [remove a branch](#remove-branch)

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
| **02** | **create & switch branch** | `git switch -c <*>` |
| **03** | **stage changes** (`.` for all) | `git add .` |
| **04** | **commit changes** | `git commit -m "*"` |

### <a id="keep-branch"></a>❯ merging code into main branch
| step | action | command |
|:---|:---|:---|
| **01** | **switch to main** | `git switch main` |
| **02** | **merge branch** | `git merge <*>` |
| **03** | **delete old branch** | `git branch -d <*>` |

### <a id="remove-branch"></a>❯ removing a branch
| step | action | command |
|:---|:---|:---|
| **01** | **switch to main** | `git switch main` |
| **02** | **force delete branch** | `git branch -D <*>` |
