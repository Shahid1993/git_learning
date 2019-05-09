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

## [Tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging)

#### List all tags
```shell
git tag --list
#or
git tag -l
# or
git tag
# for listing a particular series of tags
git tag -l "v1.8.5*"
```

#### Creating Tags
##### Annotated Tags
```shell
git tag -a v1.4 -m "my version 1.4"
```
##### Lightweight Tags
```shell
git tag v1.4-lw
```


#### Show Tag Data
```shell
git show v1.4
```

#### Sharing Tags
```shell
git push origin <tagname>.
# To Push all tags at once
git push origin --tags
```


#### Delete list of tags
```shell
git tag --list 'v-*' | xargs -I % echo "git tag -d %; git push --delete origin %" | sh
```

#### Delete a tag
```shell
# delete local tag '12345'
git tag -d 12345
# delete remote tag '12345' (eg, GitHub version too)
git push origin :refs/tags/12345
# alternative approach
git push --delete origin tagName
git tag -d tagName
```

#### Tagging Later
To tag that commit, you specify the commit checksum (or part of it) at the end of the command:
```shell
 git tag -a v1.2 9fceb02
 ```


## Git Log
```shell
git log --pretty=oneline
```








