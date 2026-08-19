# Git Exercises

1) Initialize and make first commit

- `git init`
- Create `hello.py` and commit:
  - `git add hello.py`
  - `git commit -m "chore: add hello script"`

2) Create a feature branch

- `git checkout -b feature/greet`
- Edit `hello.py` to add a function and commit.

3) Switch back and make another change on `main`

- Edit `feature.txt` and commit on `main`.

4) Merge feature branch into `main` (fast-forward or no-fast-forward)

- `git checkout main`
- `git merge feature/greet`

5) Conflict exercise

- Create a conflicting change: modify the same lines in `feature.txt` on `main` and `feature/greet`, then attempt to merge and resolve the conflict.

6) Undoing and history

- Practice `git revert`, `git reset --soft`, and `git reflog` to recover commits.

7) Tags and releases

- `git tag -a v0.1 -m "v0.1"`

8) Interactive rebase (advanced)

- `git checkout feature/greet`
- `git rebase -i main`

9) Stash and apply

- `git stash save "WIP: experiment"`
- `git stash pop`

10) (Optional) Simulate remotes

- Create a GitHub repo, then `git remote add origin ...` and `git push -u origin main`.

Use `git status` and `git log --oneline --graph --all` frequently.
