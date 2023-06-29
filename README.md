# Git management from terminal

## Generic setup
1. install git on pc
2. create shh-keygen on pc
3. upload to github profile
4. clone repos with shh method (allows pushes)
5. open folder in vscode and save changes

## Push files to origin
1. git add README.md //replace README.md with your file name
2. git commit -m "Some description of update" //describe the changes
3. git push //add files to origin

### Push more stuff
1. add folder: git add my_folder
2. add all current folder: git add .


### Conflict pushing files that already have been edited
Error sample:
 ! [rejected]        main -> main (fetch first)
error: push di alcuni riferimenti su 'github.com:matteoamorth/git-test.git' non riuscito

To force the commit:
git push --force origin main

## Remove file 
1. git rm ./my_folder/file_tmp.txt

## Pull files 

git pull
git pull --force
Check changes: git fetch

## Branches
### current branch
git branch

### New branch
Create (forced)
git checkout -b develop

### switch branch
git checkout "name"
git switch "name"

### aggiungere branch
git push origin develop

### Add the stuff in develop to the main branch (append not merging)
git push origin develop:main