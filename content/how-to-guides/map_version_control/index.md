+++
title = 'Map Version Control'
date = 2024-08-15T15:02:54+01:00
draft = false
+++

Version controlling your maps is as simple as using git!

If you don't know how to use git, here's a brief overview:

1. Install git on your computer with the following command on windows: `winget install git.git`
1. Create a directory somewhere on your computer where you'll store your project's ,map files
1. Go to github.com or gitlab.com and create a new repository in your account (create an account if you don't have one)
1. Open a terminal
1. Navigate to the directory you created in step 2 with the `cd` command
1. Run `git init` to initialize a new git repository
1. Run `git add .` to add all the files in the directory to the repository
1. Run `git commit -m "Initial commit"` to commit the files to the repository
1. Run `git remote add origin <url>` to add a remote repository. This will be explained in the repository you created in step 3
1. Run `git push -u origin HEAD` to push the files to the remote repository

That's it! Now you can version control your maps and collaborate with others on your projects. 

When you've made a change to your .map file, you can run `git add .`, `git commit -m "Your commit message"`, and `git push` to push the changes to the remote repository.
