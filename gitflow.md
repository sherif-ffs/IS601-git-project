**Git Flow**

A set of guidelines developers can follow when using version control.

Referred to as branching model.

**Git FLow Working

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



