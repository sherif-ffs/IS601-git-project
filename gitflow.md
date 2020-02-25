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

**Feature Branches :

•	New development (new features, non-emergency bug fixes) are built in feature branches.
•	Feature branch uses develop as its parent branch.
•	When feature is complete, it gets merged back into develop branch when they are ready for release.
•	It shouldn’t interact directly with the master branch.

**Release branches:

o	When it is time to make a release, a release branch comes into action and it is created off of develop.
o	Only bug fixes, documentation generation and other release oriented tasks are performed by release branch.
o	When develop has acquired enough features for release, we can fork a release of develop.
o	Once it is ready to ship, release branch gets merged into master.

**Git

Git is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

Git has three main states that your files can reside in: modified, staged, and committed:
•	Modified means that you have changed the file but have not committed it to your database yet.
•	Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
•	Committed means that the data is safely stored in your local database.

**Identity

The first thing we should do when we install Git is to set your user name and email address. This is important because every Git commit uses this information.

**Editor
			
We can configure the default text editor that will be used when Git needs you to type in a message. If not configured, Git uses your system’s default editor.

**Checking the settings

If you want to check your configuration settings, you can use the git list command to list all the settings Git can find at that point.

**Working collaboratively on github:

**Adding a collaborator 

Go to the homepage of GitHub or click here to see the following screen.

At the right top, you have this + icon, clicking on it will open up this drop-down window and add  in some basic details like the organization name, Email ID, etc.


2**Forking 

A fork is nothing but a copy of the repository. 
Forking a repository allows you to freely experiment with changes without affecting the original project.
In the homepage of your organization’s project, you can see a button named, “Fork” in the right top.

When we fork the repo we just created in the organization, it will ask under which account we want to create this fork. 
Click on your account where do you see the username and the profile picture. We will get the copy of your organization’s repo. It's called the fork of the organization's repo.

3**Cloning

When we create a repository on GitHub, it exists as a remote repository. We can clone your repository to create a local copy on your computer and sync between the two locations.


**Steps for cloning:

1. On GitHub, navigate to the main page of the repository.

2. Under the repository name, click Clone or download.

3.To clone the repository using HTTPS, under "Clone with HTTPS", click. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click.

4. Open Git Bash.

5. Change the current working directory to the location where you want the cloned directory to be made.

6. Type git clone, and then paste the URL you copied in Step 2

7. Press Enter. Your local clone will be created.
