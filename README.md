# my_git_project
Example project created for "Jump Start Git"

This project has been created for the exercises given in the Sitepoint publication "Jump Start Git" by Shaumik Daityari from August 2015.

I am working through this book using Linux Mint 19 installed on my HP Pavilion x360 Convertible laptop and will log my progress and notes in this README.md file.

***
## Chapter 2 Getting Started with Git

Installed Git (`$ sudo apt install git`) and set up some global Git variables which help to identify the user. Also set up Git Autocomplete using script available from GitHub site.

Created a working folder (repository), moved into the folder and, with the `$ git init` command set up Git to work in that repository.

Created 3 simple text files (my_file, myfile2, myfile3) ready for first stages of Git processing. The `$ git status` command shows these files as red as they are "untracked".

Used Git to add these files to the tracking system: `$ git add my_file myfile2 myfile3`. The `$ git status` command now shows these files as green as they are "tracked" and ready to be committed.

Then made a commit with these files: `$ git commit -m "First Commit"`.

Then made some simple text changes to 2 of the files, and the `$ git status` command shows these files as red as they have been changed. The `$ git diff` command shows the changes that have been made. *This step is important to make sure that the changes made were the changes wanted.*

After reviewing the changes, the new versions of the files need to be "staged" for the next commit: `$ git add my_file myfile2`. Alternatively, all tracked files can be added with: `$ git add -u`.

Then made a second commit with: `$ git commit -m "Made changes to two files"`.

The commit history can be shown by: `$ git log`. This also shows the hash codes for each commit, so more detail can be found by adding at least the first 4 characters of the hash to the log command.

(Section on using the **.gitignore** file, but not used here.)

Last section is on setting up with GitHub and pushing to a new, remote repository online. For initial set up, once an account has been created on GitHub, use: `$ git remote add origin https://github.com/jdmcclymont/my_git_project.git`. Then push the changes: `$ git push -u origin master`.

The push command sends the commits from the local repository to the cloud repository. The -u option stands for “upstream”. It links the local repository to an upstream repository for future reference. When commits are added later, Git will show the
status of the local copy in relation to the upstream repository. The **master** here signifies the files to be synchronized.

***

## Chapter 3 Branching in Git

