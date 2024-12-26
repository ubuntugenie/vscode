
```sh
grep -Ril 'text' .
```

```sh
git checkout --orphan new-branchname


git add -A


git commit -am "Initial commit"


git branch -D branchname


git branch -m branchname


git push -f origin branchname
```

```sh
git fetch origin
git reset --hard origin/master
git pull origin maste
```


```sh
# Method 1: Create and checkout an orphan branch (completely empty, no history)
git checkout --orphan new-branch-name
git rm -rf .
```
```sh
# Method 2: Create and checkout a new branch, then empty it
git checkout --orphan new-branch-name
git reset --hard
git commit --allow-empty -m "Initial empty commit"
```
The main difference:
Method 1 creates a truly empty branch with no history
Method 2 creates a branch with an empty initial commit
Most people use Method 1 when they want a completely fresh start. After either method, you can start adding new files to your branch.
Remember to replace new-branch-name with your desired branch name.
