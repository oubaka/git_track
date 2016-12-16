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
18. find the differences between "merge" and "rebase" in above cases:
19. Use git stash:
20. create a repository on github for your working repository and push changes on remote repository:

# Exercise 2
1. Create two folders project1 and project2.
2. Switch to project1 and create a repository in it named test_project.
# cd test_project
# git init
3. Switch to a new branch - 'staging'.
# git checkout -b staging
4. Add a file in it - 'test1' and add content to it 'This is first commit'.
5. Push it to github.
6. Move to folder project2.
7. Clone the repo in project2.
8. Switch to staging.
9. Change the text in file 'test1' to 'This is second commit'.
10. Commit and push to remote branch.
11. Move to project1.
12. Switch to staging branch.
13. Change the text in file 'test1' to 'This is third commit'.
14. Commit and push to remote branch. (Explain what happened here).
15. Switch to master.
16. Merge staging branch into master.
17. Create a new branch testing.
18. Change the text to 'A is an alphabet' and commit.
19. Repeat the 'step 18' seven times and each time update the alphabet 'A' to 'B' to 'C' etc.(Don't forget to commit the change everytime)
20. Push the branch to github.
21. Checkout to master.
22. Change the text '1 is a number' and commit.
23. Repeat the 'step 22' seven times and each time update the number '1' to '2' to '3' etc.(Don't forget to commit the change everytime)
24. Push master branch to github.
25. Now, rebase testing into master(and don't push the new master and testing branch).
26. Move to project2.
27. Track testing branch.
28. Checkout to master.
29. Merge branch testing into master.