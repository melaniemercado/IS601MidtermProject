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

<imgsrc="https://lh3.googleusercontent.com/8LC3KQCLgPb9U_Jh08R382c0D_UqtP_3L82O5fMi1Jg_ypoTB7B2BUk-jfB3O4C5BuGEPiE9Qcs" width=900>


**Gitflow** is a lightweight, branch-based workflow that supports projects where deployments are made regularly. The gitFlow allows you and your team to work faster and smarter.

Here is a high-level summary of the workflow:

<img src="https://lh3.googleusercontent.com/uNFxizMXUo9QAih-JVGVLPv7K_5j2wzFTSTDguPJhhQrJLk8SZcevKm4gUyLuF8rOx8LkhN6UyI" width=1100>

We will cover all stages of deployment in this tutorial. 

## Commit

A commit records a snapshot of all the files and changes made in your directory. It also maintains a history of which commits were made and when. Committing to your local repository basically acts like a buffer between your contributions and the central repository. Only once you're ready, can you then interact with the central repository.

In terminal, you can achieve this by entering: $ git commit

In the visual shown below, a commit looks as simple as another recorded snapshot of changes or "C2" 

<img src="https://lh3.googleusercontent.com/4W5_UgA3GTftLRcE_WhJBaovioDrUt9fhNgsK-n2P3cv-91rUz5__HdE35MtpSglzblAOkNjYYQ" width=400>
