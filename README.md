# gitPractice
In this task I implemented gitflow workflow by creating main and develop branches also by creating 2 feature branches, release branch and hotfix
and resolved merge conflict.

In this task firstly main branch was created.

Then I used:
git flow init command to start working.
develop branch was created.
git branch - to check available branches.
Then I created simplePage feature branch:
git flow feature start feature_branch
And added html page to it. And pushed to the remote repository:

![photo_2024-03-16_01-03-16](https://github.com/KKatiaa/gitPractice/assets/53976746/6aebf140-ef0d-4250-a197-9c4e7bd35b61)

Then I created secondPage feature branch:

![photo_2024-03-16_01-04-40](https://github.com/KKatiaa/gitPractice/assets/53976746/8c06b3ab-2720-4b05-b611-3f5e1f9a6be7)

I added changes to branch secondPage on github remote repository and on local branch and faced merge conflict
 which was successfully resolved.
git flow feature pull origin secondPage - to get new changes from remote branch.
 
![photo_2024-03-15_22-54-10](https://github.com/KKatiaa/gitPractice/assets/53976746/d13cccf7-b876-4f1f-aeb1-97901cdb9dc2)
 
Then I created release branch to make a release of the project.
And also fixed one bug on release branch from develop branch. Then I pushed released branch to develop and main branches.
After that I created hotfix branch from main branch added some changes to it and again pushed changes to both develop
and main branches.

Also I had some issues doing this so I was needed to reset my commits and restore files with commands and I used cherry-pick to pushchanges to 2 branches:
git reset --hard 1c865c54235f760788797e38d66c4714dae73e10
git restore --staged secondPage.html
git restore secondPage.html
git cherry-pick 1c865c54235f760788797e38d66c4714dae73e10

You can also check commit history on branches like secondPage.