
Git Branching, Merging & Conflicts — Quick Reference
Branching
git switch -c feature-login   # create & switch to new branch
git switch feature-login      # switch to existing branch

Merging
git switch main               # go to main branch
git merge feature-login       # merge feature branch into main
git branch -d feature-login   # delete merged branch

Merge Conflicts

Git shows <<<<<<< HEAD ... ======= ... >>>>>>> branch if same line changed

Fix manually, then:

git add file.txt              # mark conflict resolved
git commit                    # complete merge

Check Status
git status                    # see staged, unstaged, and conflicts
git log --oneline --graph --all  # visualize branches and merges


💡 Memory Trick:

Switch → branch

Merge → combine branches

Conflict → edit + add + commit
