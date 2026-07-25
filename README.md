# ╔═══════════════════════════╗
# ║     GIT CHEAT SHEET       ║
# ╚═══════════════════════════╝

> a quick-reference guide for getting your local code onto github.

### ❯ quick start table

| step | action | command |
|:---|:---|:---|
| **01** | **initialize** (skip if cloned) | `git init` |
| **02** | **connect remote** | `git remote add origin https://github.com/hcg-leo/<repo_name>` |
| **03** | **set branch** | `git branch -M main` |
| **04** | **stage files** (`.` for all) | `git add .` |
| **05** | **commit** | `git commit -m "<your_message>"` |
| **06** | **push** | `git push -u origin main` |

---

### ❯ detailed breakdown

**`git init`**
> creates a new, empty git repository. think of it as turning on tracking for your local folder.

**`git remote add origin <url>`**
> tells your local folder exactly where to send files on github.

**`git branch -M main`**
> sets your default working branch to `main`.

**`git add .`**
> moves files to the staging area. the `.` means "everything in this directory." replace `.` with a specific directory or filename if you only want to save certain files.

**`git commit -m "<message>"`**
> takes a permanent snapshot of your staged files. always leave a clear message so future-you knows exactly what you changed!

**`git push -u origin main`**
> uploads your committed changes up to github. the `-u` flag remembers your setup, so next time you can usually just type `git push`.

---------------------------------------------------------
// git //
