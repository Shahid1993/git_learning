# create a new repository on the command line
```shell
echo "# git_learning" >> README.md  
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin https://github.com/Shahid1993/git_learning.git
git push -u origin master
```
# push an existing repository from the command line
```shell
git remote add origin https://github.com/Shahid1993/git_learning.git
git push -u origin master
```

# Cloning a Git repository
#### CLONE OVER HTTPS:
```shell
 git clone https://username@bitbucket.org/teamsinspace/documentation-tests.git
```
#### CLONE OVER SSH:
```shell
 git clone ssh://git@bitbucket.org:teamsinspace/documentation-tests.git
```
#### Add all new files:
```shell
git add --all
```

#### Remove a file:
```shell
git rm <filename>
```

#### Commit changes:
```shell
git commit -m '<commit_message>'
```

#### Get an idea of the git command to use next:
```shell
git status
```

## Push updates to a repository
```shell
git push origin master
```


