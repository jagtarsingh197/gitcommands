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

