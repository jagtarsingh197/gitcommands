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

