```bash
sudo apt update
sudo apt install git gh
git --version
gh --version
```

- `git --version` prints the installed Git version.
- `gh --version` prints the installed GitHub CLI (`gh`) version.

Set the name and email Git uses to identify your commits:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

```bash
git config --list
```

- `git config --list` displays the Git configuration settings currently in effect.

Clone the GitHub repository and check its current state:

```bash
git clone https://github.com/jagtarsingh197/gitcommands.git
```

- `git clone` downloads a copy of the repository to your computer.

Enter the cloned folder, then check its current state:

```bash
cd gitcommands
git status
```

- `git status` shows the current branch and whether there are uncommitted changes.

## Git's four areas

Git organizes changes across four areas:

1. **Working directory** - the local files you view and edit.
2. **Staging area** - the changes selected to be included in the next commit.
3. **Local repository** - committed changes stored in your local Git repository.
4. **Remote repository** - the shared repository hosted on GitHub or another Git server.

```text
Working directory --> Staging area --> Local repository --> Remote repository
        ^                                                    |
        +------------------------ git pull ---------------------+
```

### Working directory

Edit project files in the working directory. Use `git status` to see modified or untracked files.

```bash
git status
```

### Staging area

Add changes from the working directory to the staging area:

```bash
git add <file>
git add .
git status
```

Use `git restore --staged <file>` to remove a file from the staging area while keeping its working-directory changes.

### Local repository

Create a commit from the staged changes and store it in the local repository:

```bash
git commit -m "Describe the changes"
git log --oneline
```

### Remote repository

Send local commits to the remote repository:

```bash
git push
```

Download changes from the remote repository and update the local branch:

```bash
git pull
```

Create an additional branch, switch to it, and push it to the remote:

```bash
git branch additional-commands
git switch additional-commands

git push --set-upstream origin additional-commands
```

