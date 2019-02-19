

# GITFLOW

## What is it?
Git-Flow is a branching methodology. It is not a silver bullet to solve all the source control questions out there, but it helps a lot if it is very well followed, specially when scattered teams and projects are pushing code into the same repository, solving most of the concurrent work that may result on code inconsistencies or conflicts.

## How to use it?
For starter, you don't need any special tool. Just knowing how to handle different situations following this paradigm.

## Learning by example
The best way to learn anything (at least in my opinion) is using it.
Some use cases and situations you may face and how to solve them using Git-Flow:

**Branching and Merging**
All in one overview of branching and how code splits and merges from branch to branch:
![Git flow workflow - Hotfix Branches](branching_overview.svg)

### Rebasing
Rebasing is useful when...

### Releases and Tags
In the previous image you can see tags (as in releases or versions) represented as baby-blue squares.
Using Github there are multiple ways of generating new releases or versions, but one of the easiest is actually tagging code at certain point. Usually either on master branch or production branch depending on the agreed semantics.

### Features
How can I separate features using the right branching?

### Work in Progress
What do I do if I have work in progress I don't know to merge into the release branch or develop branch just yet?

### Hotfixes
What should I do if I detect in production a bug and it needs to be fixed ASAP?




## Resources and tutorials:

https://nvie.com/posts/a-successful-git-branching-model/

https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
