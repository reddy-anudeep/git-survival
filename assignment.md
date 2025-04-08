Assignment 2: "Split it up" Drama
Goal: Two commits — one for readme.md, one for todo.txt.

git add readme.md
git commit -m "Update readme, ugh"
git add todo.txt
git commit -m "Add todo, whatever"



Assignment 3: "Switch Branches, Oh Crap"
Goal: Changes in todo.txt, can’t commit, must stash.

git stash
git checkout feature
git checkout tempo 
git stash list     
git stash apply    
git add todo.txt
git commit -m "Saved my bacon"



Assignment 4: "Client Wants It Online"
Goal: Push your local repo to GitHub

git remote add origin https://github.com/reddy-anudeep/git-survival.git
git branch -M main
git push -u origin main



Assignment 5: "Feature Creep" Fiasco
Goal: Create feature branch, add coolstuff.txt, merge into main.

git checkout -b feature
echo "This better work" > coolstuff.txt
git add coolstuff.txt
git commit -m "Add coolstuff feature"

git checkout main
git merge feature
git push origin main

Assignment 6: "Steal Their Code" Fork Debacle
Goal: Fork, set upstream, fetch and merge upstream

git remote add upstream https://github.com/octocat/Spoon-Knife.git
git fetch upstream
git merge upstream/main



Assignment 8: "Reviewer Hates Your History" Rewrite
Goal: Squash messy commits into one on bugfix

git checkout bugfix
git rebase -i HEAD~3

git push --force



Assignment 9: "Merge Conflict Hell"
Goal: Conflict in readme.md, resolve it, commit.

git checkout main
git commit -am "I’m the best."

git checkout feature
git commit -am "No, I’m the best."

git checkout main
git merge feature   


git add readme.md
git commit -m "Resolved merge conflict in readme.md"
