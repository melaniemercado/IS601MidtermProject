## gitFlow Tutorial

In order to understand Git, it's important to go over some key terms - version control system, distributed version control system, and repository.

#### What's a **version control system (VCS)**? 
 A version control system is a tool that helps developers manage changes to code over time. It keeps track of every modification to the code in any time of database. If a mistake is made, developers can look into earlier versions of the code to help fix the mistake and minimize disruption to other team members.
 
#### What's a **distributed version control system (DVCS)**? 
A distributed version control system emulates the same idea as VCS with one big difference -  every developer can have their own local repository without needing to have a connection to the central repository to commit. All your changes are recorded to your local repository so you have full access to every file, branch, and iteration of the project. You can essentially collaborate  anywhere and anytime. **Git** is a perfect example of a DVCS.

#### What's a **repository**?
A repository encompasses the entire collection of files and folders associated with a project, along with each file's revision history. The history appears as snapshots of changes over time, also called committees, and organized into multiple lines of development called branches. As Git is a DVCS, anyone who owns a copy of the repository can access the entire codebase and history, cloning, branching, committing, merging, comparing changes of versions, and more. 

>We will review cloning, branching, merging, etc. in more detail later in this tutorial

Here is an example of a Git repository:

<img src="https://lh3.googleusercontent.com/EgVLZcjyrH0Nfj6AxuNQ_K_cPUsKy_m-l9ZWR-cF_P_kCasORThgyq4-G_wsrxtDLzrU0Cy9_2U" width=600>


**Gitflow** is a lightweight, branch-based workflow that supports projects where deployments are made regularly. The gitFlow allows you and your team to work faster and smarter.

Here is a high-level summary of the workflow:

<img src="https://lh3.googleusercontent.com/uNFxizMXUo9QAih-JVGVLPv7K_5j2wzFTSTDguPJhhQrJLk8SZcevKm4gUyLuF8rOx8LkhN6UyI" width=1100>

We will cover all stages of deployment in this tutorial. 

## Commit

A commit records a snapshot of all the files and changes made in your directory. It also maintains a history of which commits were made and when. Committing to your local repository basically acts like a buffer between your contributions and the central repository. Only once you're ready, can you then interact with the central repository.

In terminal, you can achieve this by entering: $ git commit

In the visual shown below, a commit looks as simple as another recorded snapshot of changes or "C2" 

<img src="https://lh3.googleusercontent.com/4W5_UgA3GTftLRcE_WhJBaovioDrUt9fhNgsK-n2P3cv-91rUz5__HdE35MtpSglzblAOkNjYYQ" width=400>


## Branch

Let's say you're doing some work on a website and your employer tells you there's an urgent fix that needs to be applied on a different section of the website. You don't need to deploy your fix or put a lot of effort to revert your changes. All you have to do is switch to the production master branch, create a branch to make your changes, merge the branch, and deploy to production. Then you can switch back to your branch and continue your own work. 

In terminal, you can achieve this by entering: $ git branch [nameofbranch]

In the visual below, the new branch named "newImage" now refers to "C1", eg. $ git branch newImage

<img src="https://lh3.googleusercontent.com/-W8nMI1o8RgjXOy_f_6OLgBZUQjlA5XEp3-RN3f_JbGyJrlowtm35jTGdKHNaZ38-pPnzBoGhz8" width=400>


## Merge

Merging allows you to take independent lines of development created by $ git branch and integrate them, mostly likely back to the master branch or central repository. For example, let's say you branched off the master to make some changes to the website and you're ready to integrate your changes. The commit on the branch you're on won't be a direct ancestor of the branch you're merging into so Git has to do some work around this. Basically, Git will create a new commit that points to this merge

In terminal, you can achieve this by entering: $ git merge [nameofwork]

In the visual below, the new branch named "bugFix" in "C2" refers to your changes and "C4" refers to Git creating the new commit merging changes, ie. $ git merge bugFix.

<img src="https://lh3.googleusercontent.com/J-fvRTCK_f3SQJoF3_ZxvSrHfoPdhnZ_wOvYJN9BnTp8u5ESMo51D2QvyvOWRGAcbcf5x7fO81A" width=400>


## Checkout

The git checkout command lets you move between the branches after you used git branch. Think of it as a way to select which line of development you're working on. Do remember - Git won't let you checkout another branch or move to another branch unless your working directory is clean. You would lose any changes that you do not commit.

In terminal, you can achieve this by entering: $ git checkout [nameofwork].

In the visual below, by using the checkout function, branch "bugFix" is now moved to the same commit as master is attached to.

<img src="https://lh3.googleusercontent.com/O93DHncA4BeBt3y3k1dCZrELVxr63S2z_XCJcFtLW5G0ZgZGw2pEXuZTOuv0z0LWkyza-vOXMrM" width=400>


## Clone

Very simply put - git clone allows you to create local copies of remote repositories. Generally, cloning is a one-time operation. Once you obtain a copy, all version control operations and changes are managed through the local repository.

In terminal, you can achieve this by entering: $ git clone

In the visual below, the commits on the left indicate your local repository and on the right indicates your remote repository. The image on the left shows "o/master" which demonstrates that both your local and remote repository are a mirror image of the other.

<img src="https://lh3.googleusercontent.com/EeCHc7Rl-ZS6HtTWlN_y7Dj501pD1nI3DCu84Am_B-KDj8wue-noKZPNrKmRB4N8hfiEPbhyF4Q" width=400>


## Pull

Whereas cloning is normally used as the initial copy of a remote repository to create a local repository, the pull function allows you to update your local with any changes that occurred after the initial copy you did of the remote repository. It can also be seen as a merge of remote changes into your local repository.

In terminal, you can achieve this by entering: $ git pull [remote]

In the visual below, the left side represents your local directory. The pull function fetches "C3" commit not currently in your local repository. In order to merge the changes from remote, a new master commit "C4" appears and changes your origin/master to the latest data fetched.

<img src="https://lh3.googleusercontent.com/c5ZP1S37b_U_HkP-xYWstAKqH7NY6rfg7HxyPVgUzMhGc0Nkq-p4QqdcsJDwGMe5U31fGlUPBpQ" width=400>


## Push

The push command is used to upload local repository content to a remote repository. Whereas fetching imports commits to local branches, pushing exports commits to remote branches. This is how you publish your work.

In terminal, you can achieve this by entering: $ git push [remote] [branch] or for example, $ git push origin master

In the visual below, simply put, your left side represents your local repository in which "C2" represents your current state. On the right side, the remote was at the "C1" commit but after using the push function, now has a "C2" commit as well. This represents that your local origin/master and the remote are in sync.

<img src="https://lh3.googleusercontent.com/WzeHZzOjiMi_FGdzPhnuMqzGM5PRqMDoIw58g_RGvx-pD_tdOcaX21jJKcwQ9QHeNCwpkVmuios" width=400>


## Fork

A fork  is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.
You might fork a project in order to propose changes to the upstream, or original, repository. In this case, it's good practice to regularly sync your fork with the upstream repository. 

<img src="https://lh3.googleusercontent.com/PRUR_BDZuRnOgGXoSyiIgicSgd9mq6PPRlFkzTmIPXH6R250QSlXBBhyjx9vfWJqAUR12GCprlc" width=700>


## Remote Add / Remove / Show

<img align="right" width="350" height="290" src="https://lh3.googleusercontent.com/JVWMnHgkLdQu_IbyLLrZVy2pzwOxLl_abSNEfw1gkicUTRS4bzxhjfH0_bhPmZ2aaNeJDXSWG4Q">

The remote command lets you create, view, and delete connections to other repositories. Remote connections are more like bookmarks rather than direct links into other repositories. 

To show a remote repository, you can run $ git ls-remote.

To add a new remote Git repository as a shortname you can reference easily, run $ git remote add < shortname > < url >.

<img src="https://lh3.googleusercontent.com/-_FIhmZ-m47A6LyMW4dSgEjvySJcGUJ-nuUXP3_T-VIo4a-PMNEtl5gPgvho3URkAvf0v5NhA-k" width=400>



If you want to remove a remote for some reason — you’ve moved the server or perhaps a contributor isn’t contributing anymore — you can either use $ git remote remove or $ git remote rm. Once you delete the reference to a remote this way, all remote-tracking branches and configuration settings associated with that remote are also deleted.

<img src="https://lh3.googleusercontent.com/9Wenq25CGbDfVZP7uX4CV9_1pv5XA_iXUTPFP006EAuSKAeTrv7MN5l7uFE2FCKhRe2LpwgHb0c" width=400>


## Status

The git status command can be used to explore the state of the staging area and pending commit.

The command checks the status and reports that there’s nothing to commit, meaning the repository stores the current state of the working directory, and there are no changes to record.

It's good practice to check the state of your repository before committing changes so that you don't accidentally commit something you don't mean to. This example displays the repository status before and after staging and committing a snapshot:


<img src="https://lh3.googleusercontent.com/eYZqOj5aNUAJ_vvydRFOrFPZI8iJ8gGk-dcEb404d92JFp9b-9NktE178ri8tXyx7I8W0zKs-SI" width=500>



