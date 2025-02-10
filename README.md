# **GIT - GITHUB**

## Local Repositories

### Basic Commands

#### * git --help

Shows the help menu.

```bash
git --help
```

#### -git init

Initializes a git repository.

```bash
git init
```

#### git config

Configures git.

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

#### git status

Shows the status of the repository.

```bash
git status
```

#### git add

Adds a file to the staging area.

```bash
git add <file>
```

#### git rm

Removes a file from the staging area.

```bash
git rm --cached <file>
```

#### git commit

Commits the staged changes.

```bash
git commit -m "Commit message"
```

#### git log

Shows the commit history.

```bash
git log
git log main..origin/main # Shows the commit history between the main branch and the origin/main branch
```

### Advanced Commands

#### git branch

Creates a new branch.

```bash
git branch # Shows the current branch
git branch <branch-name> # Creates a new branch
git branch -D <branch-name> # Deletes a branch
```

#### git checkout or git switch

Switches to a branch.

```bash
git checkout <branch>
git switch <branch>
```

#### git checkout (Certain commit)

Switches to a certain commit to make changes for testing.

```bash
git checkout <commit Identifier>
git checkout -b <branch> <commit Identifier> # Creates a new branch
git checkout main # Switches to the main branch
```

#### git merge

Merges a branch into the current branch.

```bash
git merge <branch>
git merge origin/main # Merges the origin/main branch into the current branch
```

#### git rebase

Rebases a branch into another branch.

#### git revert

Reverts a commit.

```bash
git revert <commit Identifier>
```

#### git reset

Resets the current branch to a previous commit.

```bash
git reset --soft <commit Identifier> # Soft reset
git reset --mixed <commit Identifier> # Mixed reset
git reset --hard <commit Identifier> # Hard reset
```

#### git stash

Stashes the current changes.

#### git tag

Tags a commit.

```bash
git tag -a <tag-name> -m "Tag message" # Creates a tag
git tag <tag-name> # Creates a tag
git show <tag-name> # Shows the commit associated with a tag
git tag -d <tag-name> # Deletes a tag
```

#### git reflog

Shows the commit history.

## Remote Repositories

### Remote Basic Commands

#### create ssh key

```bash
ssh-keygen -t rsa -b 4096 -C "your@email.com" # Creates an rsa key
ssh-keygen -t ed25519 -C "your@email.com"  # Creates an ed25519 key
eval "$(ssh-agent -s)" # Evaluates the ssh key
ssh-add ~/.ssh/id_rsa # Adds the key to the ssh-agent
ssh -T git@github.com # Tests the connection
```

#### git remote

Manages remote repositories.

```bash
git remote add origin <url>
```

#### git clone

Clones a repository.

```bash
git clone <url>
```

#### git push

Pushes the commits to the remote repository.

```bash
git push origin <branch>
```

#### git pull

Pulls the commits from the remote repository.

```bash
git pull origin <branch>
```

##### git fetch

Fetches the commits from the remote repository.

```bash
git fetch origin <branch>
```

### Working with Branches

#### git diff

Shows the differences between the current state and the last commit.
