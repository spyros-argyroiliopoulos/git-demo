Some slides
---------------------------------------------------------
00. Theory


Explain git init. Git is working through diffing files at the filesystem
---------------------------------------------------------
0.0 spyros clone repo
0.1 chris clone project


Basic push-pull functionality
---------------------------------------------------------
1.0 show git local changes panel (intelliJ)
1.1 spyros commit on master
1.2 show commit is present local but not in remote / Github

2.0 spyros push to remote
2.1 show commit also on remote

3.0 chris show commits are not present
3.1 chris pull master
3.2 show commits are present on chris local

4.0 spyros commit and push on master
4.1 show chris local is not updated

5.0 chris pull master
5.1 show commit is present on chris master

6.0 chris commit and push to master
6.1 spyros pull and show log history (intelliJ)
6.2 examine the changes of each commit, show commit hash
6.3 show git annotate (intelliJ)

7.0 chris commit and push to master
7.1 spyros commit and push to master, push is rejected, why? branch is back
7.2 spyros pull from master and resolve conflict
7.3 spyros push the resolved commit
7.4 show on Github the commit is there


How to avoid constant conflicts, is there a better way? New branch from master.
---------------------------------------------------------
8.0 spyros checkout new branch from master
8.1 spyros commit in branch
8.2 spyros checkout master
8.3 show last commit is not there
8.4 chris fetch. show no other branches exist.
8.5 spyros push new branch in remote
8.6 chris pull from master, show no changes
8.7 chris fetch, show new branch is there
8.8 chris checkout new branch, show commits are there
8.9 chris checkout master

9.0 chris commit in master. show no conflicts
9.1 spyros commit in branch, show no conflicts
9.2 spyros open a new PR on github, show github UI, explain what is going to happen
9.3 show that PR has conflicts
9.4 spyros pull master in branch, resolve conflicts
9.5 spyros push resolved in branch
9.6 show PR has no conflicts on github, accept PR
9.7 spyros fetch, show master has incoming commits, pull master
9.8 show git log (intelliJ) all commits exist in master

> Explain git flow, the usage of branches for parallel efficient workflow

What if something goes bad? How to go back? Should I do it even if I can? What are the consequences?
---------------------------------------------------------
10.0 spyros create new branch from master
10.1 spyros commit and push in remote
10.2 spyros commit and push in remote
10.3 chris checkout branch
10.3 spyros reset head soft to previous commit, show changes are perisited but uncommited
10.4 spyros commit and FORCE push to remote, show what happened
10.5 chris pull from branch, show what happened
10.6 spyros reset hard to previous commit, show changes are lost
10.7 spyros commit and FORCE push to remote, show github
10.8 chris pull, show HEAD is on previous commit, try to push, push is rejected, either delete or git reset soft to perserve changes and push again.

> Push forward mentality, don't do force push on remote branches
> Don't checkout branch from branch


Cherrypick
---------------------------------------------------------
11.0 spyros create new branch from master
11.1 cherrypick commit from other branch, show commit is present on new branch


Branch from a specific commit, not necessarily HEAD
---------------------------------------------------------
12.0 spyros create branch from specific commit
12.1 show git log (intelliJ)


Reword commit message
---------------------------------------------------------
13.0 show reword modal
13.1 show git log (intelliJ)

Compare branch modal
---------------------------------------------------------
14.0 show compare modal
