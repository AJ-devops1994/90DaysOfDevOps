git branch: branch is an independent line of code that lets you work on features or fixes without affecting the stable main code until changes are merged after proper testing.

Why do we use branches instead of committing everything to `main`?
- in main branch stable code base is there and if multiple people will make changes at the same time then there are chances of:
	-Introduce bugs
	-Break builds
	-Cause conflicts
	-Deploy unstable code
-to keep your main code base safe and production ready all the time, it is suggested that every contributor can create there own branch to make their respective changes and after proper testing that your code is working as expected changes can be merged to main branch


What is `HEAD` in Git?
- HEAD is a pointer to current branch and in turn points to the latest commit of the current branch

What happens to your files when you switch branches?
- When switching branches, Git updates the working directory to reflect the latest commit of the selected branch.

What is the difference between clone and fork?
- clone is a copy of your remote repository on your local machine
- fork is a copy of some other remote repository to your remote repo.

When would you clone vs fork?
clone: used to copy your remote repository on your local machine
fork: used to create your own remote copy of someone else’s repository so you can modify it independently.

After forking, how do you keep your fork in sync with the original repo?
- You keep your fork in sync by fetching changes from the original repository (upstream) and merging them into your fork

What is the difference between `git fetch` and `git pull`?
- git fetch: Downloads commits, branches, and tags from a remote to your local repository without changing your working branch, used when you want to review changes before integrating
- git pull: Downloads commits from a remote and immediately merges them into your current branch, used when you want to immediately update your branch with remote changes
