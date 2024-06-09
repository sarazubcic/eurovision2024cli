Dodavanje GIT repozitorija na GitHub:

# Prvo napravimo GitHub racun, na njemu novi repozitorij i novi token za rat s Git CLI alatom
# Repozitorij URL:



git init -b main

git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

git diff --name-only --cached
# Provjeravamo koje to datoteke smo pripremili za COMMIT

git commit -m "Inicijalni commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.

git remote add origin https://github.com/sarazubcic/eurovision2024cli.git
# Povezivanje lokalnog GIT repozitorija na GitHub repozitorij

git push -u origin main
# Slanje podataka na GitHub repozitorij
