# gitFlow

GitFlow is a branching model that allows work on a project from multiple while keeping a pristine “master” branch that does not get touched (merged back into) until all features, fixes, and testing for a release.

From the beginning a project a “develop” branch is created from “master” and they will run parallel forever. All work is done off of this develop branch while the master is left alone as the finished product branch.

![Parallels](/images/Parallels.png)

Developers will branch “features” off of the develop branch. They will also fix known bugs in these feature branches. These features can be earmarked for a specific upcoming release or they can just linger out there as works in progress. As features are completed, they are merged back into the develop branch.

![Features](/images/Features.png)

Once all the features for a particular release are merged into develop the feature branch can be deleted. Then a "release" branch comes off of the develop branch. It will go through testing and only bug fixes are performed in this branch. Once a release is ready to go into production it is merged into master and back into develop and can be deleted. By doing this, only completely developed and tested releases are merged into the master branch.

![Release](/images/Release.png)
