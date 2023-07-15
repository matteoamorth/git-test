# Git management from terminal

## Generic setup
1. install git on pc
2. create shh-keygen on pc
3. upload to github profile
4. clone repos with shh method (allows pushes)
5. open folder in vscode and save changes

## Push files to origin
```bash
git add . 
git commit -m "Some description of update" //describe the changes 
git push //add files to origin
``` 

### Push specific branch
```bash
git push origin develop
```

### Add files in a branch to the main
```bash
git push origin develop:main
```

### Push only specific folders or files
```bash
git add my_folder
git add README.md
```

### Push files that already have been edited online
```bash
Error sample:
 ! [rejected]        main -> main (fetch first)
error: push di alcuni riferimenti su 'github.com:matteoamorth/git-test.git' non riuscito
```

To force the commit:
```bash
git push --force origin main
```

## Remove file 
To remove file "file_tmp.txt" in "my_folder"
```bash
git rm ./my_folder/file_tmp.txt
```

Remove all
```bash
git rm -r --cached .
```

## Pull files 
```bash
git pull
git pull --force
```

Check changes:
```bash
git fetch
```

## Branches
### Look current branch and branches list
```bash
git branch
```

### New branch
Create (forced)
```bash
git checkout -b develop
```

### Switch branch
```bash
git checkout "name" 
git switch "name"
```

## Exclude folders from branch
create file .gitignore 

```gitignore
#FOLDER
your_folder/

#File extensions to discard
*.asv
*.bak
*.rst
```
