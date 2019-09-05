Solution to open every dir in a git folder that contains a repository. 
Script will change every branch to master and make a pull request

```
git_parent_folder="git"

for dir in $git_parent_folder/*;
do
    for subdir in $dir/*;
    do
      cd $subdir;
      git checkout master; git pull;
    done
done
```
