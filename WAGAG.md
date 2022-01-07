# What is Git and what is GitHub ? 

***

### Summary of Git

**Git** is ***Version Control System (software) for tracking changes in any set of files*** , used for coordinating work among programmers collaboratively developing source code during software development.

It tracks the history of changes as people and teams collaborate on projects together. As developers make changes to the project, any earlier version of the project can be recovered at any time.

Every Git directory on every computer is a full-fledged **repository** with complete history and full version-tracking abilities, independent of network access or a central server. Git is free and oper-source.

Developers can review project history to find out:

* Which changes were made?
* Who made the changes?
* When were the changes made?
* Why were changes needed?


##### Interesting facts

Torvalds (the creator) sarcastically quipped about the name git (which means "unpleasant person" in British English slang): "I'm an egotistical bastard, and I name all my projects after myself. First 'Linux', now 'git'. The man page describes Git as "the stupid content tracker". 

The read-me file of the source code elaborates further, "git" can mean anything, depending on your mood :

* Random three-letter combination that is pronounceable, and not actually used by any common UNIX command. The fact that it is a mispronunciation of "get" may or may not be relevant.
* Stupid. Contemptible and despicable. Simple. Take your pick from the dictionary of slang.
* "Global information tracker": you're in a good mood, and it actually works for you. Angels sing, and a light suddenly fills the room.
* ***"Goddamn idiotic truckload of sh*t": when it breaks.***

### Summary of Github

##### GitHub hosts Git repositories.

**GitHub** is a ***provider of Internet hosting*** for software development and version control using *Git*. Think like "cloud" for code. Projects on GitHub can be accessed and managed using the standard Git command-line interface; all standard Git commands work with it. GitHub also allows users to browse public repositories on the site.

Users are able to have discussions, manage repositories, submit contributions to others' repositories, and review changes to code for free. 

> The fundamental software that underpins *GitHub* is *Git* itself. The main purpose of GitHub is to facilitate the version control and issue tracking aspects of software development.

What is also useful - ***GitHub Pages*** , static web hosting service offered by GitHub since 2008 to GitHub users for hosting user blogs, project documentation, or even whole books created as a page.

##### Interesting facts

From 2012, Microsoft became a significant user of GitHub, using it to host open-source projects and development tools such as .NET Core, Chakra Core, MSBuild, PowerShell, PowerToys, Visual Studio Code, Windows Calculator, Windows Terminal and the bulk of its product documentation. 6 years later, Microsoft bought GitHub, however, it continued to operate independently as a community, platform and business.

***
## Key phrases

### Pull, Commit

For version control, Git (and by extension GitHub) allows **pull requests** to propose changes to the source code. Users with the ability to review the proposed changes can see a diff of the requested changes and approve them. In Git terminology, this action is called **committing** and one instance of it is a **commit** , which can be explained as *a snapshot in time*. A history of all commits is kept and can be viewed at a later time.

### Repository or *Repo*, Branches

A **repository**, or Git project, stores the entire collection of files and folders associated with a project, along with each file's commits. The commits can be organized into multiple lines of development called **branches**.

Using the terminal, a Git repository also allows for: interaction with the history, cloning the repository, creating branches, committing, merging, comparing changes across versions of code, and more.

***

## Basic Git commands

Along with already known commands like ls, rm, cd ,pwd, mkdir,cp, rmdir etc , in Git Bash users use :

* ***git init***  initializes a brand new Git repository and begins tracking an existing directory. It adds a hidden subfolder within the existing directory that houses the internal data structure required for version control. ( .git )
* ***git clone*** creates a local copy of a project that already exists remotely. The clone includes all the project's files, history, and branches. 
        *git clone <https://name-of-the-repository-link>*
* ***git add*** stages a change. Git tracks changes to a developer's codebase, but it's necessary to stage and take a snapshot of the changes to include them in the project's history. 
        *git add <file> or -A for all*
* ***git commit*** saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that's been staged with git add will become a part of the snapshot with git commit. 
       *git commit -m "commit message"*
* ***git status*** shows the status of changes as untracked, modified, or staged.
* ***git branch*** shows the branches being worked on locally.  To create a branch locally , *git branch <branch-name>*. To push the new branch into the remote repository 
        *git push -u <remote> <branch-name>*
* ***git merge*** merges lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the main branch for deployment.
* ***git pull*** updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment. This command is a combination of git fetch and git merge which means that, when we use git pull, it gets the updates from remote repository (git fetch) and immediately applies the latest changes in your local (git merge).
* ***git push*** updates the remote repository with any commits made locally to a branch. git push --set-upstream origin main ,pushes changes to github

Good to know : 

 * git checkout , switches branches 
 * git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git , provides the path for the repository you created on github
* git log -- oneline , to see our commit history
* git revert hash code (from git log) , to revert changes





***

##### More information, useful links: 

[GitHub about Git + examples](https://docs.github.com/en/get-started/using-git/about-git)


### Testing GIT and Github

Added new text, now commit and Push :)))