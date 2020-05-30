**GITFLOW BRANCHING MODEL**

Every new development starts in the *feature* branch, where the developers begin building the code.

![Step One](https://datasift.github.io/gitflow/GitFlowFeatureBranches.png)

*Feature* branch is branched off of the *develop* branch to merge the completed coding components back to the *develop* branch for the release.

![Step Two](https://datasift.github.io/gitflow/GitFlowDevelopBranch.png)

Once the code is ready for release, the *release* branch is created off of the *develop* branch.

![Step Three](https://datasift.github.io/gitflow/GitFlowReleaseBranch.png)

Code begins its testing in the *release* branch, and examine for any problems to get fixed. It goes into the *deploy* --> *test* --> *fix* --> *redeploy* --> *retest* cycle on repeat until it is suitable enough for consumers to use. Once ready, it will merge into the *master* and *develop* branches to preserve the updated code from any accidental deletions.

![Step four](https://datasift.github.io/gitflow/GitFlowMasterBranch.png)
   
*Master* branch only has the released code; commits are only merges from the *release* and *hotfix* branches.

![Step five](https://datasift.github.io/gitflow/GitFlowHotfixBranch.png)

*Hotfix* branch is for emergency fixes, which are branched off of the *master* branch. When finished, it merges to the *develop* and *master* branches to also preserve the updated code from any accidental deletions.

**Reference**

* Driessen, Vincent. “Introducing GitFlow.” Introducing GitFlow, 2015, datasift.github.io/gitflow/IntroducingGitFlow.html.
