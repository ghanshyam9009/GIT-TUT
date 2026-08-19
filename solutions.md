# Solutions / Reference Commands

1) Init & first commit

```
git init
git add hello.py
git commit -m "chore: add hello script"
```

2) Feature branch

```
git checkout -b feature/greet
git add hello.py
git commit -m "feat: add greet()"
```

3) Make a change on main

```
git checkout main
git add feature.txt
git commit -m "docs: update feature notes"
```

4) Merge

```
git checkout main
git merge feature/greet
```

5) Resolve conflict example

When merge reports conflicts, open the conflicted file, edit to resolve, then:

```
git add feature.txt
git commit -m "fix: resolve merge conflict in feature.txt"
```

6) Undoing

```
git revert <commit>
git reset --soft HEAD~1
git reflog
```

7) Tag

```
git tag -a v0.1 -m "v0.1"
git show v0.1
```

8) Interactive rebase

```
git checkout feature/greet
git rebase -i main
```

9) Stash

```
git stash save "WIP: experiment"
git stash list
git stash pop
```
