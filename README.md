# Git management from terminal

## Generic setup
1. install git on pc
2. create shh-keygen on pc
3. upload to github profile
4. clone repos with shh method (allows pushes)
5. open folder in vscode and save changes

## Push files to origin
1. git add .
2. git commit -m "Some description of update" //describe the changes
3. git push //add files to origin

### Push specific branch
git push origin develop

### Add files in a branch to the main
git push origin develop:main

### Push more stuff
1. add folder: git add my_folder
2. add only a file: git add README.md


### Push files that already have been edited online
Error sample: <br>
 ! [rejected]        main -> main (fetch first)
error: push di alcuni riferimenti su 'github.com:matteoamorth/git-test.git' non riuscito

To force the commit:
git push --force origin main

## Remove file 
To remove file "file_tmp.txt" in "my_folder" <br>
git rm ./my_folder/file_tmp.txt
Remove all <br>
git rm -r --cached .

## Pull files 

git pull <br>
git pull --force <br>
Check changes: git fetch <br>

## Branches
### Look current branch and branches list
git branch

### New branch
Create (forced) <br>
git checkout -b develop

### Switch branch
git checkout "name" <br>
git switch "name"


## Exclude folders from branch
create file .gitignore

Sample <br>
#FOLDER
your_folder/

#Files extension to discard
*.asv
*.bak
*.rst

