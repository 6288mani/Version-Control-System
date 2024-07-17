# Version Control Systems

# What is a “version control system”? 

Version control systems are a category of software tools that helps in recording changes made to files by keeping a track of modifications done in the code. 

# Why Version Control system is so Important?

As we know that a software product is developed in collaboration by a group of developers they might be located at different locations and each one of them contributes to some specific kind of functionality/features. So in order to contribute to the product, they made modifications to the source code(either by adding or removing). A version control system is a kind of software that helps the developer team to efficiently communicate and manage(track) all the changes that have been made to the source code along with the information like who made and what changes have been made. A separate branch is created for every contributor who made the changes and the changes aren’t merged into the original source code unless all are analyzed as soon as the changes are green signaled they merged to the main source code. It not only keeps source code organized but also improves productivity by making the development process smooth.
Basically Version control system keeps track on changes made on a particular software and take a snapshot of every modification. Let’s suppose if a team of developer add some new functionalities in an application and the updated version is not working properly so as the version control system keeps track of our work so with the help of version control system we can omit the new changes and continue with the previous version.

# Benefits of the version control system:

* Enhances the project development speed by providing efficient collaboration,
* Leverages the productivity, expedites product delivery, and skills of the employees through better communication and assistance,
* Reduce possibilities of errors and conflicts meanwhile project development through traceability to every small change,
* Employees or contributors of the project can contribute from anywhere irrespective of the different geographical locations through this VCS,
* For each different contributor to the project, a different working copy is maintained and not merged to the main file unless the working copy is validated. The most popular example is Git, Helix core, Microsoft TFS,
* Helps in recovery in case of any disaster or contingent situation,
* Informs us about Who, What, When, Why changes have been made.

# Use of Version Control System: 
* A repository: It can be thought of as a database of changes. It contains all the edits and historical versions (snapshots) of the project.
* Copy of Work (sometimes called as checkout): It is the personal copy of all the files in a project. You can edit to this copy, without affecting the work of others and you can finally commit your changes to a repository when you are done making your changes.
* Working in a group: Consider yourself working in a company where you are asked to work on some live project. You can’t change the main code as it is in production, and any change may cause inconvenience to the user, also you are working in a team so you need to collaborate with your team to and adapt their changes. Version control helps you with the, merging different requests to main repository without making any undesirable changes. You may test the functionalities without putting it live, and you don’t need to download and set up each time, just pull the changes and do the changes, test it and merge it back. It may be visualized as. 

# Types of Version Control Systems: 
* Local Version Control Systems
* Centralized Version Control Systems
* Distributed Version Control Systems

# Local Version Control Systems:
  It is one of the simplest forms and has a database that kept all the changes to files under revision control. RCS is one of the most common VCS tools. It keeps patch sets (differences between files) in a special format on disk. By adding up all the patches it can then re-create what any file looked like at any point in time. 

# Centralized Version Control Systems:
  Centralized version control systems contain just one repository globally and every user need to commit for reflecting one’s changes in the repository. It is possible for others to see your changes by updating. 
    Two things are required to make your changes visible to others which are:  

  * You commit
  * They update

![image](https://github.com/user-attachments/assets/98db236d-8640-4912-8468-03aa5686985e)

The benefit of CVCS (Centralized Version Control Systems) makes collaboration amongst developers along with providing an insight to a certain extent on what everyone else is doing on the project. It allows administrators to fine-grained control over who can do what.
It has some downsides as well which led to the development of DVS. The most obvious is the single point of failure that the centralized repository represents if it goes down during that period collaboration and saving versioned changes is not possible. What if the hard disk of the central database becomes corrupted, and proper backups haven’t been kept? You lose absolutely everything.

# Distributed Version Control Systems:
Distributed version control systems contain multiple repositories. Each user has their own repository and working copy. Just committing your changes will not give others access to your changes. This is because commit will reflect those changes in your local repository and you need to push them in order to make them visible on the central repository. Similarly, When you update, you do not get others’ changes unless you have first pulled those changes into your repository.
To make your changes visible to others, 4 things are required:  

    You commit
    You push
    They pull
    They update
The most popular distributed version control systems are Git, and Mercurial. They help us overcome the problem of single point of failure.  

![image](https://github.com/user-attachments/assets/f720f96e-a956-465e-8064-931152efa0d6)

# Purpose of Version Control: 
* Multiple people can work simultaneously on a single project. Everyone works on and edits their own copy of the files and it is up to them when they wish to share the changes made by them with the rest of the team.
* It also enables one person to use multiple computers to work on a project, so it is valuable even if you are working by yourself.
* It integrates the work that is done simultaneously by different members of the team. In some rare cases, when conflicting edits are made by two people to the same line of a file, then human assistance is requested by the version control system in deciding what should be done.
* Version control provides access to the historical versions of a project. This is insurance against computer crashes or data loss. If any mistake is made, you can easily roll back to a previous version. It is also possible to undo specific edits that too without losing the work done in the meanwhile. It can be easily known when, why, and by whom any part of a file was edited.
# Centralized Version Control VS Distributed Version Control Systems

![349412036-316d0af7-e169-409d-97ff-6bce94e0b60d](https://github.com/user-attachments/assets/36b01181-8d05-4f33-8527-1eae5b35a92b)

# GIT VS GITHUB

![image](https://github.com/user-attachments/assets/5f184ca6-fc01-497c-800a-1474210d2a7f)

![image](https://github.com/user-attachments/assets/c05be20c-5c50-42f9-b094-8ed0c9012f54)

# Life-Cycle of GIT

![image](https://github.com/user-attachments/assets/1ce9eaf8-c110-4985-a928-1890b575cd95)

# GIT Branching Strategy
To add some feature funcationalities without distrubing the existing main funcationalities branching strategy is used.
  *  Better Practice for Real Time Branching Strategy as follows: -
    
      * Feature Branching : It is created for New funcationalities.
      * Release Branching : It is created for Testing purpose & Delivery.
      * Hotfix Branching : It is created for addressing bugfix in production.
      * Main Branching : It is used for existing funcationalities.

# GIT Commands
# GIT Configuration & Set-up :
  * git config –global user.name “Your Name” :- Used to Set your username globally.
  * git config –global user.email “youremail@example.com” :- Used to Set your email globally.
  * git config –global color.ui auto – :- Used to Set to display colored output in the terminal.
  * git config -list :- Used to list all environment variables of git.
  * git help :- Used to Display the main help documentation, showing a list of commonly used Git commands.
# GIT Initializing a Repository :
  * git init :- Used to Initialize a new Git repository in the current directory.
  * git init <directory> :- Used to Create a new Git repository in the specified directory.
  * git clone <repository_url> :- Used to Clone a repository from a remote server to your local machine (to Download from URL).
  * git clone –branch <branch_name> <repository_url> :- Used to Clone a specific branch from a repository.
# GIT Basic Commands :
  * git fork :- Used to copy the repository for one developer remote server to another devloper remote server.
  * git add * [file] :- Adds one or more files to the staging area.
  * git commit -m "message" [file] :- Records or snapshots the file permanently in versioning.
  * git commit -a [file] :- commits any files you have added with git add command and commits any files you have changed since then.
  * git commit -a -m "message" [file] :- Adds files to staging and versioning.
  * git status :- It lists all the files that have to be committed.
  * git diff :- Shows the file difference which are not yet staged.
  * git diff -staged :- Shows the difference between the files in the staging area & latest version.
  * git diff [branch1] [branch2] :- Shows the difference between two branches.
  * git reset [file] :- Unstages the file, but it preserves the file content.
  * git reset [commit] :- Undos all the commits after the specified commit & preserves the changes locally.
  * git reset -hard [commit] :- Discards all history and goes back to specified commit.
  * git rm [file] :- Deletes the file from your working directory & stages the delection.
  * git log :- Used to list the version history for current branch.
  * git log -follow [file] :- Lists version history for a file, include renaming of files also.
  * git show [commit] :- Shows the metadata & content changes of the specified commit.
  * git tag [commit] :- Used to give tags to the specified commit.
  * git branch :- Lists all the local branches in the current repository.
  * git branch [branch_name] :- Creates a new branch with specified branch_name.
  * git branch -d [branch_name] :- deletes the branch of specified branch_name.
  * git checkout [branch_name] :- Used to switch from one branch to another branch.
  * git checkout -b [branch_name] :- Creates a new branch of specified branch_name & also switchs to that branch
  * git remote add [variable_name] [Remote_server_link] :- Used to connect local to remote server.
  * git push [Variable_name] [branch_name] :- Sends that specified branch commits to remote repository server.
  * git push -all [Variable_name] :- Sends all branchs to remote repository server.
  * git push [Variable_name] : [branch_name] :- Deletes a specified branch on your remote repository server.
  * git pull [repository_link] :- It Fetches & Merges changes on the remote server to your local working directory. which is nothing but [git fetch + git merge].
  * git fetch :- Used to track remote branching to your local working tree.
  * git merge [branch_name] :- It merges the specified branch history to current branch.
  * git rebase [branch_name] :- Linear changes from one branch to another branch as merge.
  * git cherry-pick [branch_name] :- Non-Linear changes from one branch to another branch as merge.
  * git stash :- It stores the unstaged git add changes.
  * git stash save :- Temporarily stores all the modified tracked files.
  * git stash pop :- Restores the most recently stashed files.
  * git stash list :- Lists all stashed changesets.
  * git stash drop :- Discards the most recently stashed changeset.
  * git blame [file] :- Information about each line modification done by author.
