# git-crash-course
This is a small little repo I use to crash course my friends through using git! 

It will start out with a blank example.txt file, which will be updated through the course of this simple tutorial.

In the section below, T will refer to tutor and S will refer to student.

Basics:

1. Cloning a repo
Desc: Clone this repo!
S: Run 'git clone' to clone the repo

2. Pulling the latest changes
Desc: Pulls changes from origin into your local file system
T: Insert "This is a new line added in example.txt", commit and push the change
S: Run 'git pull' to merge the changes locally

3. Branching
Desc: Switch to and create branches
S: 
- Run 'git branch -a' to view all branches (make sure to git pull first so you have the latest branches!)
- Run  'git branch *branch name* to create a new branch based off your current branch
- Run 'git checkout *branch name* to switch to *branch name*
- (Above commands can be combined to 'git checkout -b *branch name*)
- All your commits will now be pushed to this branch

4. Staging changes and pushing them to remote repository
Desc: Keep track of local changes and push a commit once ready
S: 
- Insert 1 line of change into example.txt
- Run 'git status' to see changed files and 'git diff' to view changes
- Run 'git add .' to stage all modified files or 'git add *path to file*' to stage that particular file 
- Run 'git commit' or 'git commit -m' to commit your changes 
- Run 'git log' to see the commit history and verify that you have made the right changes
- Run 'git push' to push your changes to the remote repository
Here is a good resource to learn about writing good commit messages https://chris.beams.io/posts/git-commit/
TL:DR
- Up to 50 characters recommended, 72 maximum
- Capitalise the first letter of the message
- Do not end the message with a full stop
- Write in the imperative mood (i.e. message must fit in this sentence: "If applied, this commit will *your commit message*")
- Explain what and why things were changed instead of how

5. Merging
Desc: Merge the changes from your branch into another branch
- Switch to the target branch (the one you want your changes to be reflected on, e.g. master)
- Run 'git merge *branch name*'
- The commits from *branch name* will be added to master
- Remember to 'git push' to push your changes to the remote repository