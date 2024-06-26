# Connect Downloaded Zip to Git Repo

some times it is not possible to use command (( clone )) to connect to the remote git repository, for example because the repository is very large and timeout occur in (( clone )) process. to solve this problem one method is to download zip format of the source files from git repository manually and unzip it in our local computer, then connect it to the remote git repository where we downloaded it from. so after downloading and unzipping, do the following steps respectively:

1. git init
2. git remote add origin [git source remote URL]
3. git add .
4. git pull origin master 

from now on, you can work with your connected local git repository as usual.



***

# revert local changes

to revert local changes run the following commands:

- git reset
  - This will un-stage all files you might have staged with `git add` 
- git checkout .
  - This will revert all local uncommitted changes (should be executed in repo root).
  - run `git checkout [some_dir|file.txt]` to revert uncommitted changes only to particular file or directory.



following command will remove all local untracked files, so *only* git tracked files remain:

- git clean -fdx
  - `-x` will also remove all ignored files like `.gitignore`.



Another way to revert all uncommitted changes (longer to type, but works from any subdirectory)

- git reset --hard HEAD