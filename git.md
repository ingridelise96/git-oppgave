## Sette opp git lokalt

git init

git add .

git remote add origin https://github.com/ingridelise96/git-oppgave.git

git commit -m "initial commit"

git push -u origin master

touch .gitignore && echo "node_modules" > .gitignore

## Lage dev-branch og legge til hiof.js

touch hiof.js

git checkout -b dev

git add hiof.js

git commit -am "initial dev"

git push --set-upstream origin dev

## Hente inn endringer fra remote til local

git fetch

git pull

## Merge fra dev til master

git merge dev

git push

## Lager og resolver merge conflict

git add .

git commit -m "merge conflict test"

git push

git pull

git add .

git commit -m "resolved merge conflict"

git push