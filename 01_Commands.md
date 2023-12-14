# Add to Git

when already there is a folder (for example d:\prj1) which contains some content, and you want to add it to a git repository, do the following steps respectively:

1. open git bash in directory (( d:\prj1 ))
2. run command (( git init )).
   - this command will create git infrastructure in directory (( d:\prj1 )). 
3. run command (( git remote add origin [URL to the remote repository] ))
   - this command specifies the git source repository that you want to work with.
   - example: git remote add origin https://github.com/hamedvalizadeh/git-tutorial.git



# Upload First Time

if there is no files in the remote source repository and you want to upload your local files to it for the first time, do the following steps respectively:

1. follow steps is section (( Add to Git )).
   - after completing this section, you will have a local git repository that is connected to the remote source repository with a default branch named (( master )).
2. run the command (( git add --all ))
   - this command with stage all the changes in local repository (these changes are all files that contains in your local working directory).
3. run the command (( git commit -m "your commit message" ))
4. run the command (( git push --set-upstream origin [the name of current local branch] ))
   - example: git push --set-upstream origin master



***



# Change Repository

in order to change the current git source repository to some new one run the command (( git remote set-url [new URL to the remote repository] ))

- example:  git remote set-url https://github.com/hamedvalizadeh/git-tutorial.git





***



