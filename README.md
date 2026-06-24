# Git-learning
Its about how Im learning git until now and all the things I've learnt until now.

Git is a content addressable file system:
In its name we can find out that it contains or store all the files and datas with its key values where it has its own unique key values where it has its own unique cryptographic hash values where it can denote some duplication files or storage according to the duplication or integrity.
The term integrity means that the only the authoraized people are able to access that files.If some unauthorized people are trying to access the file,the term integrity wont be there and the case of duplication might come too.

The core component beind it are:
Blob:Its main work is to store the raw file content,it derives the key values from the data,not the file name.
We can find the hash values in the .git/objects
If we make some changes on our code and commit it,the blob object doesn't only keep the files that are changed in git,it entirely takes all the content of a file and make a new content of a file with the new hash files.

Tree:It is a type of git object where it allows to stores all the working directories and files in a single project or repository,along with a hash values for each files and directories along with the unique identifier for each files and directories.

Commit:It is a type of git object where it takes the snapshot of the working directory at a particular time.Git it divided at two phases:Adding the code to our staging area and committing it.
It records the status of the tracked file,along with its author,timestamp and messages too.

2. Essential Git Commands References:
   Settting up and initialization:
   Creating a new repository for github:
   git init.

   Configuring our global Identity by:
   git-cinfig --global user.name "Bidhanshu Bhandari"
   git-config --global user.email "bidhanshu2002@gmail.com".

   # Check the status of your working directory and staging area
git status

# Add a specific file to the staging area
git add <file-name>

# Add ALL modified and new files to the staging area
git add .

# Permanently record your staged changes into local history
git commit -m "feat: add user authentication feature"

# Upload your local commits to the remote repository
git push origin <branch-name>

# Fetch and download latest changes from remote and merge them into your current branch
git pull origin <branch-name>

Branching and Merging Strategies:
# List all local branches (current branch has an asterisk *)
git branch

# Create a new branch
git branch <new-branch-name>

# Switch to an existing branch
git checkout <branch-name>
# (Alternative modern command): git switch <branch-name>

# Create and switch to a new branch in a single command
git checkout -b <new-branch-name>
# (Alternative modern command): git switch -c <new-branch-name>

# Merge another branch into your CURRENT active branch
git merge <branch-to-merge-from>

This line is from main branch
