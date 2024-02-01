## Git command Cheatsheet

# basic terminal command
cd <directory>
touch <filename>
mkdir <foldername>
rm -r <filename>

# Repo initialize
git init

# common command
git add .   (move to staging phase)
git rm 0f <filename>    (delete file in repo)
git commit -m "<message>"  (command for complete the staging phase)
git log     (show repo's log)
git status  (show repo status in the staging phase)

git log --oneline (simplify the repo's log)

# versioning command
git checkout <commit-id>    (move the file to selected version/timeline)
git revert <commit-id>      (revert the file to selected version/timeline)
git reset --hard <commit-id>    (reset the file to selected version/timeline)

# create .gitignore.txt file to untrack certain file/ auto generated file
touch .gitignore
git rm -r --cached . (remove the cached if the tracking still working)
(Messages: put the name of the files or folder into the text file as an example, "<filename>" or "<foldername>/*" the asterick represent to ignore every file in the folder)