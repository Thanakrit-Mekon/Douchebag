# Git cheatsheet

## Basic usage

Git Initialization

```bash
git init
```

Git add everything

```bash
git add .
```

Git commit message

```bash
git commit -m "Message"
```

Git push

```bash
git push
```

Get all branches

```bash
git branch --all
```

Switching branches

```bash
git checkout my_branch
```

Create new branch

```bash
git checkout -b my_branch
```

Return to previous branch

```bash
git checkout -
```

Find commit SHA

```bash
git log
```

Switch to specific commit

```bash
git checkout SHA
```

## Add remote repository

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/Thanakrit-Mekon/Douchebag.git 
git push -u origin main
```
