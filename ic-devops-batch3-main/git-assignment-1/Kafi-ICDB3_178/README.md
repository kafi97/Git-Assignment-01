# GitHub Commands


## Basic git commands

Followings are the basic commands of git

## Configure git

```bash
## git configure file setup 
git config --global user.name "xyz" # your github user name
git config --global user.email "xyz99@gmail.com" # your email id
## generate ssh key
#ssh-keygen
Ssh-keygen -t rsa -b 4096 -C “xyz99@gmail.com”
##To the ssh-key we have to go root directory
cd ~
Cd .ssh
Cat id_rsa.pub
## Here id_rsa is public key and id_rsa is the private key
## Valid check by both public + private key
## Add this publickey content to https://github.com/settings/keys with a name
## Check connection
Ssh -T git@github.com

```
## Initialize a git repository


```bash
#Initialize a repository in a project folder:
 git init

```


```bash
#Add files to the repository to start tracking changes:

 git add .

```

```bash
#Commit the changes with a message describing:

 git commit -m "Initial commit"

```

## Working with Commits

```bash
# Check the files status:

 git status

``` 

```bash
# Make additional changes to files, then stage and commit again:

git add <filename>
git commit -m "Updated file"

``` 

```bash
# View commit history:

git log

``` 

## Branching and Merging




Branches let you work on different features without affecting the main

```bash
# Create a new branch:

git branch new-feature

``` 

```bash
# Switch to a branch:

git checkout new-feature

``` 

```bash
# After making changes and committing, merge the branch back to main:

git checkout main
git merge new-feature

``` 
## Working with Remote Repositories

```bash
# Add a remote repository:

git remote add origin https://github.com/username/repo.git

``` 


```bash
# Push changes to the remote repository:

git push -u origin main

``` 
```bash
# Push changes to the remote repository:

git pull origin main

``` 


