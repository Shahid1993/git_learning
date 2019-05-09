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

## Tags

#### List all tags
```shell
git tag --list
#or
git tag -l
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
```
git tag -d tagName

