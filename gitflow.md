**Git Flow**

A set of guidelines developers can follow when using version control.

Referred to as branching model.

**Git FLow Working**

•	Works with the help of central repository.
•	Developers can clone the central repository and can work locally.
•	They can push their branches into the central repository.
•	Two branches used to record project history.

1.	Master
2.	Develop
                 
•	Develop serves as an integration branch for features.
•	Master branch stores the official release history.

**Feature Branches**

•	New development (new features, non-emergency bug fixes) are built in feature branches.
•	Feature branch uses develop as its parent branch.
•	When feature is complete, it gets merged back into develop branch when they are ready for release.
•	It shouldn’t interact directly with the master branch.

<img src=C:\Users\ajkum\Desktop"\fb.png">

**Release branches**

o	When it is time to make a release, a release branch comes into action and it is created off of develop.
o	Only bug fixes, documentation generation and other release oriented tasks are performed by release branch.
o	When develop has acquired enough features for release, we can fork a release of develop.
o	Once it is ready to ship, release branch gets merged into master.

**Git**

Git is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

Git has three main states that your files can reside in: modified, staged, and committed:
•	Modified means that you have changed the file but have not committed it to your database yet.
•	Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
•	Committed means that the data is safely stored in your local database.

**Identity**

The first thing we should do when we install Git is to set your user name and email address. This is important because every Git commit uses this information.

**Editor**
			
We can configure the default text editor that will be used when Git needs you to type in a message. If not configured, Git uses your system’s default editor.

**Checking the settings**

If you want to check your configuration settings, you can use the git list command to list all the settings Git can find at that point.

**Working collaboratively on github**

**Adding a collaborator**

Go to the homepage of GitHub or click here to see the following screen.

At the right top, you have this + icon, clicking on it will open up this drop-down window and add  in some basic details like the organization name, Email ID, etc.


**Forking**

A fork is nothing but a copy of the repository. 
Forking a repository allows you to freely experiment with changes without affecting the original project.
In the homepage of your organization’s project, you can see a button named, “Fork” in the right top.

When we fork the repo we just created in the organization, it will ask under which account we want to create this fork. 
Click on your account where do you see the username and the profile picture. We will get the copy of your organization’s repo. It's called the fork of the organization's repo.

**Cloning**

When we create a repository on GitHub, it exists as a remote repository. We can clone your repository to create a local copy on your computer and sync between the two locations.


**Steps for cloning**

1. On GitHub, navigate to the main page of the repository.

2. Under the repository name, click Clone or download.

3.To clone the repository using HTTPS, under "Clone with HTTPS", click. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click.

4. Open Git Bash.

5. Change the current working directory to the location where you want the cloned directory to be made.

6. Type git clone, and then paste the URL you copied in Step 2

7. Press Enter. Your local clone will be created.

**Pull Request **

Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. 

Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.


When you file a pull request, all you’re doing is requesting that another developer pulls a branch from your repository into their repository. 

This means that you need to provide 4 pieces of information to file a pull request: the source repository, the source branch, the destination repository, and the destination branch.

**Steps in creating pull request**

Step 1: Fork the original project into your own GitHub account, and then clone it to your computer.

Step 2: Make a local branch for your new code.

Step 3: Create a text file and push it to the github.

Step 4: Merge your branch into master, and then delete it

Step 5: Stage. Commit. Push.

Step 6 : New pull request.

**Branching**

A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process
 
We can think of them as a way to request a brand new working directory, staging area, and project history. 

New commits are recorded in the history for the current branch, which results in a fork in the history of the project.

**Merge conflicts**

Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it.

In these cases, Git cannot automatically determine what is correct. Conflicts only affect the developer conducting the merge, the rest of the team is unaware of the conflict. 

Git will mark the file as being conflicted and halt the merging process. It is then the developers' responsibility to resolve the conflict.


**Creating a merge conflict

oCreate a new directory named git-merge-test, change to that directory, and initialize it as a new Git repo.

oCreate a new text file merge.txt with some content in it.

oAdd merge.txt to the repo and commit it

Creating a merge conflict:

Create a new directory named git-merge-test, change to that directory, and initialize it as a new Git repo.

Create a new text file merge.txt with some content in it.

Add merge.txt to the repo and commit it
Now we have a new repo with one branch master and a file merge.txt with content in it.
o	Next, we will create a new branch to use as the conflicting merge.
	create and check out a new branch named new_branch_to_merge_later
	overwrite the content in merge.txt
	commit the new content

•	With this new branch: new_branch_to_merge_later we have created a commit that overrides the content of merge.txt
•	This chain of commands checks out the master branch, appends content to merge.txt, and commits it.
•	This now puts our example repo in a state where we have 2 new commits. One in the master branch and one in the       new_branch_to_merge_later branch


•	Open the merge.txt file.
•	Once the file has been edited use git add merge.txt to stage the new merged content. To finalize the merge create a new commit by executing:
•	Git will see that the conflict has been resolved and creates a new merge commit to finalize the merge.


	Tools to resolve merge conflicts:

	git status  -- It will help identify conflicted files
	git log –merge  -- Passing the --merge argument to the git log command will produce a log with a list of commits that conflict between the merging branches.
	git diff --    diff helps find differences between states of a repository/files. This is useful in predicting and preventing merge conflicts
