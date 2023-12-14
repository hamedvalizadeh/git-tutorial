# Add to Git

when already there is a folder (for example d:\prj1) which contains some content, and you want to add it to a git repository, do the following steps respectively:

1. open git bash in directory (( d:\prj1 ))
2. run command (( git init )).
   - this command will create git infrastructure in directory (( d:\prj1 )). 
3. run command (( git remote add origin [URL to the remote repository] ))
   - this command specifies the git source repository that your want to work with.
   - example: git remote add origin https://github.com/hamedvalizadeh/git-tutorial.git