# Python Practice - Session 3

1. Create a local folder and initialize it for git;

git init -b main

2. Create a text file in the folder and commit it;

git status
git add new_file.txt
git commit -m "Add new_file"

3. Create a remote repository on GitHub;

https://github.com/SiaAnalyst/Project-test

4. Push the local repository to GitHub;

git remote add origin https://github.com/SiaAnalyst/Project-test.git
git remote -v
git push origin main

5. Create a new branch (develop) and switch to it;

git checkout -b develop

6. Create a new branch from 'develop' and switch to it;

git checkout -b feature1

7. Add the first line in the text file, commit, and push to remote;

git add new_file.txt
git commit -m "Add changes to new_file"
git push origin develop
git push origin feature1

8. Clone your repository from GitHub into a separate folder;

git clone https://github.com/SiaAnalyst/Project-test.git
cd Project-test/
 
9. Create another branch from 'develop' and switch to it using cloned project;

git checkout develop
git checkout -b feature2

10. Add the first line of the text file (different from the first branch), 
    commit, and push on remote;

git add new_file.txt
git commit -m "Add new changes to new_file"
git push origin develop
git push origin feature2

11. Switch to develop;

git checkout develop

12  Merge the first branch and push changes;

git merge feature1
git push origin feature1

13. Merge the second branch and push changes;

git checkout develop
git pull
git merge feature2
git push origin feature2

14. Resolve conflict;

Fix the file
git add new_file.txt
git commit -m "Fix conflicts"
git push

16. Commit and push a separate text file with a list of all the commands, which were used to solve the problem;
