git init
git add .
git remote add origin https://github.com/ingridelise96/git-oppgave.git
git commit -m "initial commit"
git push -u origin master
touch .gitignore && echo "node_modules" > .gitignore
touch hiof.js
git checkout -b dev
git add hiof.js
git commit -am "initial dev"
git push --set-upstream origin dev
git fetch
git pull
git merge dev
git push
git add .
git commit -m "merge conflict test"
git push
git pull
git add .
git commit -m "resolved merge conflict"
git push