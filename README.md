# Exercise 1
1. Create a repository: 
# git init
2. Make some changes -- add some files, change content of some files
3. commit changes: 
# git commit -a -m "first commit"
4. repeat steps 1-3 for 2 more times. try to remove and ignore some files . Use git diff before each commit.
5. create changes and revert those changes using git when those changes are not added to staging are: 
# git checkout -- *
6. create changes and revert those changes after adding changes to staging area: 
# git reset HEAD
7. create change and revert those changes after committing those changes : 
# git reset --hard HEAD~1
8. Check repository status before adding changes to staging area, after adding changes to staging area and after committing changes: 
# git status
9. Display all the commits: 
# git log
10. Display a specific commit: 
# git log -n 1
11. create branches called "feature1" and "feature2" from master. 11 . Delete branch "feature2": 
# git checkout master
# git branch feature1
# git branch feature2
# git branch -d feature2
12. Make some commits on "feature1":
# git checkout feature1
# git commit -a -m "add new hello text"
13. Make some commits on branch "master":
# git checkout master
# git commit -a -m "add new line of text"
14. merge branch "feature1" in "master" (make some conflicts by changing same file on same line in both the branches) 15.create branch "feature2" from master:
# git checkout master
# git merge feature1
15. Make some commits on "feature2":

16. Make some commits on branch "master":
17. rebase branch "master" in "feature2" (make some conflicts by changing same file on same line in both the branches):
# git checkout master
# git rebase feature2
18. find the differences between "merge" and "rebase" in above cases:
# The difference between merge and rebase is
# 1. Merge just applies the needed changes to the branch from which the merge was run, whereas 
# Rebase will affect the commit history by replaying the chain of commit history involved or needed
19. Use git stash:
# git stash
# git stash save
# git stash pop
# git stash drop
20. create a repository on github for your working repository and push changes on remote repository:
# git remote add origin https://github.com/oubaka/git_track.git
