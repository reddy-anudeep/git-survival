Assignment 1: "I Forgot to Track This" Crisis

Commands:
mkdir git-survival
cd git-survival
git init
echo "I'm already screwed." > README.md
git add README.md
git commit -m "Initial commit, losers"

Commit Log:
9b0fd0f (HEAD -> master) Initial commit, losers



Assignment 2: "Boss Wants It Split Up" Drama

Commands:
echo "I’m still screwed." > README.md
git add README.md
git commit -m "Update readme, ugh"

echo "Fix everything" > todo.txt
git add todo.txt
git commit -m "Add todo, whatever"

Commit Log:
8912303 Add todo, whatever
6901ae4 Update readme, ugh



Assignment 3: "It’s On Fire, Stash It!"

Commands:
echo "Almost done..." >> todo.txt
git stash

Deliverable:
git stash list
stash@{0}: WIP on master: 8912303 Add todo, whatever



Assignment 4: "The Client Wants It Online" Rush

Commands:
git remote add origin https://github.com/username/git-survival.git
git push -u origin main

Deliverable:
GitHub URL: https://github.com/username/git-survival



Assignment 5: "The Feature Creep" Branch Fiasco

Commands:
git checkout -b feature
echo "This better work" > coolstuff.txt
git add coolstuff.txt
git commit -m "Add coolstuff feature"

git checkout main
git merge feature
git push

Commit Log:
8641166 (HEAD -> main, feature) Add coolstuff feature



Assignment 6: "Steal Their Code" Fork Debacle

Commands:
git clone https://github.com/reddy-anudeep/Spoon-Knife.git
cd Spoon-Knife
git remote add upstream https://github.com/octocat/Spoon-Knife.git
git fetch upstream
git merge upstream/main

Deliverable:
git remote -v
origin    https://github.com/reddy-anudeep/Spoon-Knife.git
upstream  https://github.com/octocat/Spoon-Knife.git



Assignment 7: "My Stash Saved Me" Miracle

Commands:
git checkout -b tempo
git stash pop
git add todo.txt
git commit -m "Saved my bacon"

Commit Log:
7e11775 (HEAD -> tempo) Saved my bacon



Assignment 8: "Reviewer Hates Your History" Rewrite

Commands:
git checkout -b bugfix
echo "bug" > fix.txt
git add fix.txt
git commit -m "Bug found"
echo "oops" >> fix.txt
git add fix.txt
git commit -m "Oops"
echo "fixed again" >> fix.txt
git add fix.txt
git commit -m "Fixed again"

git rebase -i HEAD~3
git push --force

Commit Log:
Single squashed commit: Bug fix, take it or leave it



Assignment 9: "Merge Conflict Hell" Showdown

Commands:
git checkout main
echo "I'm the best" > readme.md
git commit -am "Change from main"
git checkout -b feature2
echo "No, I'm the best" > readme.md
git commit -am "Change from feature"
git checkout main
git merge feature2
git add readme.md
git commit

Commit Log:
Merge commit with conflict resolved



Assignment 10: "The Forgotten Push" Panic

Commands:
git push origin main

Deliverable:
All commits pushed and visible on GitHub

