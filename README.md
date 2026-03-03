#########################################################\
####################   Git Exercise  ####################\
##################  Git Local Practice  #################\
#########################################################

Git Local Practice

Project: Building a Simple Website (Text-Only Version)

Goal
Manage a small 'website' project with 3 files:
index.txt
about.txt
contact.txt
Each step reinforces a Git concept using a structured scenario.

Initial Setup
Objective: Create a Git repository and understand untracked and tracked files.
Instructions:
Create a folder called my-website.
Inside the folder, create three files:
index.txt (write: 'Welcome to my website')
about.txt (write: 'This site is created for Git practice')
contact.txt (write: 'Email me at example@example.com')

Run:
git init
git status
Question: Are these files tracked or untracked? **They are untracked**

Step 1: Staging Files
Objective: Learn how to stage files and the difference between staged and unstaged changes.
Instructions:
Stage index.txt:
git add index.txt
git status
Observe: One file is staged, others are still untracked.
Now stage all files:
git add .
git status


Step 2: Committing Changes
Objective: Make the first commit and understand committed files.
Instructions:
Commit all staged files:
git commit -m "Initial commit with index, about, and contact pages"
git status
Question: Are there any modified or untracked files? **No there aren't**

Step 3: Modifying Tracked Files
Objective: Understand modified vs unmodified files.
Instructions:
Edit about.txt and add: 'This is a demo project for Git.'
Run:
git status
Observation: about.txt is now modified but unstaged.

View changes:
git diff
Stage the change:
git add about.txt
View changes again:
git diff
What do you expect now?

Step 4: Unstaging a File
Objective: Learn how to unstage a file.

Instructions:
Unstage about.txt:
git restore --staged about.txt
Run:
git status


Step 5: Committing Incremental Changes
Objective: Understand smaller commits and commit history.
Instructions:
Stage and commit about.txt again:
git add about.txt
git commit -m "Updated about page with project description"
Run:
git log


Step 6: Practice Round - Combined Concepts
Scenario: Add and modify content across files to reinforce all the above concepts.
Edit all three files with something new in each.
Run git status, and identify:
Modified files
Untracked files (if you created any new ones)
Staged vs unstaged files
Use git diff and git diff --staged to inspect changes.

Try:
Staging one file
Unstaging it
Committing only one file
Leaving others uncommitted
Use git log to view the growing commit history.

Bonus: Create a New Untracked File
Objective: See how Git handles new files.
Create readme.txt with project instructions.
Run git status.
Add and commit it using the usual flow.
