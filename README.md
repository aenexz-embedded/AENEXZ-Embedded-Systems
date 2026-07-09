# AENEXZ Embedded Systems (July 2026 Batch)

Welcome! This repo is where all session submissions live for the duration of
the internship. All work happens on the **`batch/july-2026`** branch — this
is the branch you'll base your work off, and the branch your PRs must target.

## Repo structure

```
AENEXZ-Embedded-Systems/
├── README.md
├── session1/
│   ├── member1-code-sesh1.txt
│   ├── member2-code-sesh1.txt
│   └── ...
├── session2/
├── session3/
└── ...
```

Each session gets its own folder. Inside it, every student submits **one
file, uniquely named** (see naming convention below).

---

## One-time setup

Do this once, the first time you contribute.

1. **Fork this repo** — click **Fork** (top right of this page). This creates
   `your-username/AENEXZ-Embedded-Systems` under your own GitHub account.

2. **Clone your fork locally:**
   ```bash
   git clone https://github.com/YOUR-USERNAME/AENEXZ-Embedded-Systems.git
   cd AENEXZ-Embedded-Systems
   ```

3. **Add the original repo as `upstream`** (lets you pull the latest class
   content later):
   ```bash
   git remote add upstream https://github.com/aenexz-embedded/AENEXZ-Embedded-Systems.git
   ```

4. **Switch to the batch branch:**
   ```bash
   git checkout batch/july-2026
   ```

---

## Steps to submit — every session

Repeat this process for every session's assignment.

### 1. Sync with the latest class content
```bash
git checkout batch/july-2026
git fetch upstream
git pull upstream batch/july-2026
```
This avoids working on stale code and prevents unnecessary merge conflicts.

### 2. Create your own submission branch
Naming convention: `submit/<yourname>-sesh<N>`
```bash
git checkout -b submit/rahul-sesh1
```

### 3. Add your file in the correct session folder
File naming convention (strict):
```
session1/rahul-code-sesh1.txt
```

### 4. Commit your work
```bash
git add session1/rahul-code-sesh1.txt
git commit -m "Add Session 1 submission - Rahul"
```

### 5. Push to your fork
```bash
git push origin submit/rahul-sesh1
```

### 6. Open a Pull Request
- Go to your fork on GitHub -> you'll see a **"Compare & pull request"** banner. Click it.
- **Base repository:** `aenexz-embedded/AENEXZ-Embedded-Systems`
- **Base branch:** `batch/july-2026`
- **Head repository:** your fork
- **Compare branch:** `submit/rahul-sesh1`
- **PR title:** `[Session1] Rahul — submission`
- Click **Create pull request**

### 7. Wait for review
Your instructor will review and merge. Don't reuse or push further to a
branch that's already been merged. Start a fresh `submit/...` branch for
the next session.

---

## File naming convention (strict)

```
session<N>/<yourname>-code-sesh<N>.txt
```

Examples:
```
session1/rahul-code-sesh1.txt
session1/priya-code-sesh1.txt
session2/rahul-code-sesh2.txt
```

Rules:
- All lowercase, hyphens only, no spaces
- One file per person per session
- **Do not** edit, rename, or delete another student's file
- **Do not** touch files outside your own session folder submission

Following this exactly is what keeps merge conflicts from happening at all,
since every filename is unique, Git never has two people editing the same
lines of the same file.

---

## Common issues

| Problem | Fix |
|---|---|
| GitHub says your branch is "out of date" | Re-run step 1 (sync with upstream) before pushing |
| You forgot to create a new branch and committed to `batch/july-2026` directly on your fork | That's fine on your fork — just make sure your PR's compare branch is correct before submitting |
| PR shows changes from unrelated commits | You likely branched off an old `batch/july-2026` — sync with upstream and rebase, or ask for help before opening the PR |

---

Questions? Ask in the batch group before your PR deadline, don't wait
until the last minute to discover a Git issue.
