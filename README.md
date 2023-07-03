# JustGitIT
How To Git Bash To Github 

https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github#initializing-a-git-repository

(Initializing a Git repository)


Open Git Bash.

Navigate to the root directory of your project.

Initialize the local directory as a Git repository. By default, the initial branch is called main.
If you’re using Git 2.28.0 or a later version, you can set the name of the default branch using -b.
<<  git init -b main  >>

Add the files in your new local repository. This stages them for the first commit.
<<  git add .  >>
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

Commit the files that you've staged in your local repository.
<<  git commit -m "First commit"  >>
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.



(Importing a Git repository with the command line)



Create a new repository on GitHub.com. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub. For more information, see "Creating a new repository."

At the top of your repository on GitHub.com's Quick Setup page, click  to copy the remote repository URL.

Open Git Bash.

Change the current working directory to your local project.

In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
<<  git remote add origin <REMOTE_URL>  >>
# Sets the new remote

<<  git remote -v  >>
# Verifies the new remote URL

Push the changes in your local repository to GitHub.com.
<<  git push origin main  >>
# Pushes the changes in your local repository up to the remote repository you specified as the origin
