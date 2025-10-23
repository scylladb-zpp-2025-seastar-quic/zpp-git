<!-- theme: uncover -->
<!-- class: invert -->
<!-- paginate: true -->

<style>
section {
  background-image: url('scylla-logo2.png');
  background-repeat: no-repeat;
  background-position: bottom 20px left 20px;
  background-size: auto 50px;
}
</style>


# How To Use Git At Scylla Efficiently

---

# Goals of our work

- Implement features

---

# Goals of our work

- Implement features
- Make code reviews easier to perform

---

# Goals of our work

- Implement features
- Make code reviews easier to perform
- Keep changes understandable in the future

---

# Clone repository

```bash
$ git clone git@github.com:ewienik/zpp-git.git
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
$ git log --oneline
8d7ec69 (HEAD -> master, origin/master, origin/feature, origin/HEAD) Prepare initial marp presentation
e4a1d03 Initial commit
```

---

# Switch branch

```bash
$ git switch feature
branch 'feature' set up to track 'origin/feature'.
Switched to a new branch 'feature'
$ git status
On branch feature
Your branch is up to date with 'origin/feature'.

nothing to commit, working tree clean
```

---

# Create branch

```bash
$ git switch -c change-docs
Switched to a new branch 'change-docs'
$ git status
On branch change-docs
nothing to commit, working tree clean
```

---

# Create commits

```bash
$ sed -i 's/Create commits/Change branch/' use-git-at-scylla-efficently.md
$ git status
$ git add .
$ git commit -m "Change 'Create commits' slide"
$ git log --oneline
```

---

# Create commits

```bash
$ sed -i 's/Rebase with master/Sync with master/' use-git-at-scylla-efficently.md
$ git status
$ git add .
$ git commit -m "Change 'Rebase with master' slide"
$ git log --oneline
```

---

# Create commits

```bash
$ sed -i 's/Create commits/Change branch/g' use-git-at-scylla-efficently.md
$ git status
$ git add .
$ git commit -m "Change other 'Create commits' slides"
$ git log --oneline
```

---

# Rebase with master

---

# Cleanup before review

---

# Rearrange commits

---

# Split commits

---

# Update commits

---

# Push changes

---

# Rework after review

---

# Push changes

---

# Tools

```bash
$ git
$ tig
$ jj
```

