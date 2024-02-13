## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we watned to create a git repo in a new project we create the folder and the initalize that repo using `git init`
```
mkdir /Users/mac/GitHub/tmp/.git/
cd /Users/mac/GitHub/tmp/.git/
git init
touch Readme.md
open Readme.md
git status
git add .
# makes changes to readme.md
git commit -a -m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespaces we'll a create 
temporary diractory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace
```

### HTTPS

```sh
git clone https://github.com/sjsjsmsmsj/GitHub.git
cd GitHub
```

## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice. 
```
git commit
```

Set the global  editor
```
git config --global core.editor emacs
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that willbe included in the commit 
We can use the . to add all possible files.
```
git add Readme.md
git add .
```

## Reset

Reset allows you to move Staged changes to be unstaged. 
This is useful when you to revert all files not to be not commited

```
git add .
git resert
```
> git reset will revet a git add .

## Status

Git status shows you what files will or will not be commited.

```
git status
```
## Gitconfig file

The gitconfig file is what stores your global configuarations for git such as email, name, editor and more.

Showing the contnets of our .gitconfig file
```
git config --list
```

When you first install Git on a machine you are suppose to set up your name and email

```sh
git config --global user.name "LamGiaThinh"
git config --global user.email johndoe@example.com
```
