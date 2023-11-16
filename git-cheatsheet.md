## Basic Git Configuration
- `git config --global user.name "Your Name"`
  - Sets your name for commit markers.
  - Example: `git config --global user.name "Jane Doe"`
- `git config --global user.email "your_email@example.com"`
  - Sets your email for commit markers.
  - Example: `git config --global user.email "jane@example.com"`

## Creating Repositories
- `git init`
  - Initializes a new Git repository.
  - Example: Navigate to your project directory and run `git init`
- `git clone [url]`
  - Clones a repository from a URL.
  - Example: `git clone https://github.com/user/repo.git`

## Basic Snapshotting
- `git status`
  - Checks the status of your changes.
  - Example: `git status` shows modified files and files staged for commit.
- `git add [file]`
  - Stages a file for the next commit.
  - Example: `git add myfile.txt`
- `git add .`
  - Stages all changes for the next commit.
  - Example: `git add .` to add all changed files.
- `git commit -m "[commit message]"`
  - Commits the staged snapshot with a message.
  - Example: `git commit -m "Initial project commit"`

## Branching and Merging
- `git branch`
  - Lists, creates, or deletes branches.
  - Example: `git branch` to list branches, `git branch feature1` to create a branch.
- `git checkout [branch_name]`
  - Switches to a branch.
  - Example: `git checkout feature1` switches to `feature1` branch.
- `git merge [branch]`
  - Merges a branch into the active branch.
  - Example: `git merge feature1` merges `feature1` into the current branch.

## Sharing and Updating
- `git push [alias] [branch]`
  - Pushes a branch to your remote repository.
  - Example: `git push origin master` pushes the `master` branch to `origin`.
- `git pull`
  - Fetches and merges changes from the remote to your working branch.
  - Example: `git pull origin master` pulls changes from `origin` to `master`.

## Inspection and Comparison
- `git log`
  - Shows a log of commits.
  - Example: `git log` displays the commit history.
- `git diff`
  - Shows changes between commits, commit and working tree, etc.
  - Example: `git diff` shows unstaged changes.

## Undoing Changes
- `git restore [file]`
  - Discards changes in the working directory.
  - Example: `git restore myfile.txt` undoes changes in `myfile.txt`.
- `git revert [commit]`
  - Reverts some existing commits.
  - Example: `git revert 1a2b3c4` reverts commit `1a2b3c4`.
- `git reset [commit]`
  - Resets your HEAD to a previous state.
  - Example: `git reset 1a2b3c4` resets to commit `1a2b3c4`.

## Advanced Commands
- `git stash`
  - Temporarily stores modified, tracked files.
  - Example: `git stash` saves current changes temporarily.
- `git stash pop`
  - Applies stored stashed content.
  - Example: `git stash pop` applies the most recently stashed changes.

## Working with Remotes
- `git remote add [alias] [url]`
  - Adds a remote repository.
  - Example: `git remote add origin https://github.com/user/repo.git`
- `git fetch [alias]`
  - Fetches branches and/or tags from the remote.
  - Example: `git fetch origin` fetches updates from `origin`.
- `git push -u [alias] [branch]`
  - Pushes a branch to your remote repository and sets it to track the remote branch.
  - Example: `git push -u origin master` pushes `master` to `origin` and sets up tracking.
