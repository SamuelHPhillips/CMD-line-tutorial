This tutorial is primarily for Terminal (Mac OSX), but has very similar syntax for Windows CMD-line/Powershell 

After creating a directory in GitHub, open the CMD line, and use the command
git clone  https://[github repository].git

Make sure you are in the directory you want the clone to be saved in

For example, to clone this repository, use:
git clone https://github.com/SamuelHPhillips/CMD-line-tutorial.git

This creates a local 'clone' or copy of the repository as it currently is, on your machine.
Once the clone is saved locally, you can add, edit, or delete files as you'd like in your local clone.

When you're in the local directory, using the command:
git status

will return any differences between the current branch in the repository you're working on, and your local version, including:
1) modifications to existing files 2) any new (untracked) files 3) deleted files, etc.

After making changes to the local clone (while still in that directory), the command:
git add [filename]


will add the file to the online repository on the GitHub servers. 
You can also use the command:
git add -A 
to add ALL files that have been created in the local directory (useful if many files have been made).

Using git status now will show the file name, but will also tell you that the file still needs to be committed.

To do this, use the command:
git commit -n "[message]"

The -n allows you to add the "[message]", which should explain the changes that have been made in this commit. For example:
git commit -n "added file index.html"

This still hasn't saved the changes to the GitHub repository however, you still need to do one more thing.

To finalize the commit to the online repository, use the command:
git push

this "pushes" the latest commit to the GitHub repository, permenantly changing it's content. 
Now, anyone who (with file authorization) uses the command:
git pull

will "pull" the latest version of the repository, including any changes you just made. 
You must be in the local repository directory to push or pull from the GitHub repository. 

These are the most important git commands, however, simply typing 
git
while in the local repository will provide a manual of all the git commands and their effect. Check them out and give them a try!
