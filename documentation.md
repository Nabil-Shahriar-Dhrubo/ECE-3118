# **Documentation on Git Commands**

### Course No.: ECE 3118
### Course Name: Software Engineering and Information System Design Sessional

**Submitted to:**</br>
---
Rakibul Hassan</br>
Lecturer</br>
Department of Electrical and Computer Engineering</br>
RUET</br>


**Submitted by:**</br>
---
Nabil Shahriar Dhrubo</br>
Roll: 1710002</br>
Department of Electrical and Computer Engineering</br>
RUET</br>

---

# **Git**

> ***Git** is a distributed version control tool that can manage a programmer's source code history.*

 It is designed to handle minor to major projects with high speed and efficiency. It is developed to co-ordinate the work among the developers. The version control allows us to track and work together with our team members at the same workspace.

Git is foundation of many services like **GitHub** and **GitLab**, but we can use Git without using any other Git services. Git can be used privately and publicly.

![Git and Github](https://joshcannons.com/img/logo/logo-github.jpg)

# **GitHub**
> ***GitHub** is a Git repository hosting service. It is a web-based service.*

GitHub is an online service to store code and push from the computer running the Git tool. GitHub focused on centralized source code hosting.

# **Git Commands:**

Git supports many command-line tools and graphical user interfaces. The Git command line is the only place where we can run all the Git commands.

# **1. Git Configuration:**

The Git config command is the first and necessary command used on the Git command line. This command sets the author name and email address to be used with your commits. Git config is also used in other scenarios. 

**Syntax**
```
git config --global user.name "Nusrat-Jahan-ECE"  
git config --global user.email "1710011@student.ruet.ac.bd"
````
# **2. To Check Git Version:**

We can check your current version of Git by running the following command in Git Bash, terminal (Linux, macOS) or command prompt (Windows).

**Syntax:**
```
git --version
````
# **3. Git Initialization**

To create a blank repository, open command line on your desired directory and run the init command as follows:
```
git init
````
# **4. Git Status Command**

The status command is used to display the state of the working directory and the staging area. It also lists the files that you've changed and those you still need to add or commit.

**Syntax:**
```
git status
````
# **5. Git Add Command**

This command is used to add one or more files to staging (Index) area.

**Syntax:**

**i. To add one file:**
```
git add <Filename>  
````
**ii. To add more than one file:**
```
git add*
````
**iii. To add all files:**
```
git add -A
````
# **6. Git Commit Command**

This command changes the head. It records or snapshots the file permanently in the version history with a message.

![Git add vs Git commit](https://www.w3docs.com/uploads/media/default/0001/03/ad19114d2f18ae7f7e8b99a5110d1a2f339282c6.png)



**Syntax:**


```
git commit -m " Commit Message"  
````
# **7. Git Clone Command**


![Git clone](https://www.w3docs.com/uploads/media/default/0001/03/3f26b30cc1dbda3424ceef3ab4977149906a0c58.png)



This command is used to make a copy of a repository from an existing URL. If I want a local copy of my repository from GitHub, this command allows creating a local copy of that repository on your local directory from the repository URL.

**Syntax:**
```
git clone <URL> 
````
# **8. Git Push Command**

![Git push, pull, fetch](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT1w88vBx7BiiMDBhKfu9Hfmvt63pWk5YyAaE7nT-b9bUet0Fn7cG0Ae13yGm0wIDQ30TU&usqp=CAU)


It is used to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repo. It's the complement to git fetch, but whereas fetching imports commits to local branches on comparatively pushing exports commits to remote branches. 

Remote branches are configured by using the git remote command. Pushing is capable of overwriting changes, and caution should be taken when pushing.

**i. Git push origin master**

This command sends the changes made on the master branch, to our remote repository.

**Syntax:**
```
git push [variable name] master 
````
**ii. Git push -all**

This command pushes all the branches to the server repository.

**Syntax:**
```
git push --all 
````
# **9. Git Pull Command**

Pull command is used to receive data from GitHub. It fetches and merges changes on the remote server to your working directory.

**Syntax:**
```
git pull <URL>  
````
# **10. Git Fetch:**


![Git fetch](https://static.javatpoint.com/tutorial/git/images/git-fetch.png)


The "git fetch" command is used to pull the updates from remote-tracking branches. Additionally, we can get the updates that have been pushed to our remote branches to our local machines. As we know, a branch is a variation of our repositories main code, so the remote-tracking branches are branches that have been set up to pull and push from remote repository. 

**Syntax:**


**i. To fetch the remote repository:**
```
git fetch< repository Url> 
````

**ii. To fetch a specific branch:**
```
git fetch <branch URL><branch name>  
```

**iii. To fetch all the branches simultaneously:**
```
git fetch -all  
```

**iv. To synchronize the local repository:**
```
git fetch origin  
```
# **11. Git Merge Command**

![Git merge](https://docs.microsoft.com/en-us/azure/devops/repos/git/media/regular_branch_merge.png?view=azure-devops)


This command is used to merge the specified branch history into the current branch.

**Syntax:**
```
git merge  <branch-name>
````

# **12. Git Log Command**

This command is used to check the commit history.

![Git log](https://www.blog.nakulrajput.com/wp-content/uploads/2018/10/Git-Status.jpg)


**Syntax:**
```
git log
````
# **13. Git Remote Command**

Git Remote command is used to connect your local repository to the remote server. This command allows you to create, view, and delete connections to other repositories. These connections are more like bookmarks rather than direct links into other repositories. This command doesn't provide real-time access to repositories.


**Syntax:**
```
git remote add origin <URL>
````
# **13. Git Origin Master:**

The term "git origin master" is used in the context of a remote repository. It is used to deal with the remote repository. The term origin comes from where repository original situated and master stands for the main branch.

### **Git Master:**

Master is a naming convention for Git branch. It's a default branch of Git. After cloning a project from a remote server, the resulting local repository contains only a single local branch. This branch is called a "master" branch. It means that "master" is a repository's "default" branch.


![Git master](https://static.javatpoint.com/tutorial/git/images/git-origin-master.png)


In most cases, the master is referred to as the main branch. Master branch is considered as the final view of the repository.

**Syntax:**
```
git remote add origin <URL>
````

### **Git Origin:**

In Git, The term origin is referred to the remote repository where you want to publish your commits. The default remote repository is called origin, although you can work with several remotes having a different name at the same time. It is said as an alias of the system.


![Git origin](https://static.javatpoint.com/tutorial/git/images/git-origin-master2.png)


The origin is a short name for the remote repository that a project was initially being cloned. It is used in place of the original repository URL. Thus, it makes referencing much easier.

Some commands in which the term origin and master are widely used are as follows:
```
Git push origin master
``` 
```   
Git pull origin master
```
# **14. Git Branch Command**

![Git branch](https://res.cloudinary.com/practicaldev/image/fetch/s--Jc-acrrl--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/69payngupg75rqgabwdg.png)


Branches are highly important in the git world. By using branches, several developers are able to work in parallel on the same project simultaneously. We can use the git branch command for creating, listing and deleting branches.

**Syntax:**

**i. Creating a new branch:**
```
git branch <branch-name> 
````
This command will create a branch locally. To push the new branch into the remote repository, you need to use the following command:

```
git push -u <remote> <branch-name>
```
**ii. Viewing branches:**
```
git branch or git branch --list
```

**iii. Deleting a branch:**
```
git branch -d <branch-name>
```

# **15. Git Checkout Command**

![Git checkout](https://static.javatpoint.com/tutorial/git/images/git-checkout.png)


This is also one of the most used Git commands. To work in a branch, first you need to switch to it. We use git checkout mostly for switching from one branch to another. We can also use it for checking out files and commits.

**Syntax:**
```
git checkout <name-of-your-branch>
````
# **16. Git Stash:**


![Git Stash](https://static.javatpoint.com/tutorial/git/images/git-stash.png)


The git stash command enables us to switch branches without committing the current branch.

Stashing takes the messy state of your working directory, and temporarily save it for further use. Many options are available with git stash. Some useful options are given below:

**Syntax:**


**i. Git stash:**
```
git stash 
````

**ii. Git Stash Save (Saving Stashes with the message):**

In Git, the changes can be stashed with a message. To stash a change with a message, we run the below command:
```
git stash save "<Stashing_Message>"   
```

**iii. Git Stash List (Check the Stored Stashes):**

To check the stored stashes, we run the below command:
```
git stash list  
```

**iv. Git Stash Apply:**

We can re-apply the changes that you just stashed by using the git stash command. To apply the commit, we use the git stash command, followed by the apply option. It is used as: 
```
git stash apply  
```
**v. Git Stash Changes:**

We can track the stashes and their changes. To see the changes in the file before stash and after stash operation, run the below command:
```
git stash show
````

**vi. Git Stash Pop (Reapplying Stashed Changes):**

The git stash pop command is quite similar to git stash apply. The main difference between both of these commands is stash pop command that deletes the stash from the stack after it is applied.
```
git stash pop
```

**vii. Git Stash Drop (Unstash):**

The git stash drop command is used to delete a stash from the queue. Generally, it deletes the most recent stash. Caution should be taken before using stash drop command, as it is difficult to undo if once applied.

The only way to revert it is if you do not close the terminal after deleting the stash. The stash drop command will be used as:
```
git stash drop  
```

**viii. Git Stash Clear:**

The git stash clear command allows deleting all the available stashes at once. To delete all the available stashes, operate below command: 
```
git stash clear
```
**ix. Git Stash Branch:**

The git stash branch command allows the user to stash work on a separate branch to avoid conflicts. The syntax for this branch is as follows:
```
git stash branch <Branch Name>  
```

# **17. Git Revert Command**

Sometimes we need to undo the changes that we've made. There are various ways to undo our changes locally or remotely (depends on what we need), but we must carefully use these commands to avoid unwanted deletions.t

Then we just need to specify the hash code next to our commit that we would like to undo.

**Syntax:**
```
git revert <hash_code>
````


![Git revert and reset](https://64.media.tumblr.com/cde0683673e8d27c3db284e4c7965e08/tumblr_inline_mwzr3bz8fW1rk7mw6.png)

# **18. Git Reset Command**

The term reset stands for undoing changes. The git reset command is used to reset the changes. The git reset command has three core forms of invocation. These forms are as follows:


- Hard
- Mixed
- Soft (Head)

### **i. Git Reset Hard:**

It will first move the Head and update the index with the contents of the commits. The --hard option changes the Commit History, and ref pointers are updated to the specified commit. 

Then, the Staging Index and Working Directory need to reset to match that of the specified commit. Any previously pending commits to the Staging Index and the Working Directory gets reset to match Commit Tree. It means any awaiting work will be lost.

**Syntax:**
```
git reset --hard 
````
### **ii. Git Reset Mixed:**

A mixed option is a default option of the git reset command. If we would not pass any argument, then the git reset command considered as --mixed as default option. 

A mixed option updates the ref pointers. The staging area also reset to the state of a specified commit. The undone changes transferred to the working directory.

**Syntax:**
```
git reset --mixed 
````
### **iii. Git Reset Head (Git Reset Soft):**

The soft option does not touch the index file or working tree at all, but it resets the Head as all options do. When the soft mode runs, the refs pointers updated, and the resets stop there. It will act as git amend command. It is not an authoritative command. Sometimes developers considered it as a waste of time.

Generally, it is used to change the position of the Head. Let's understand how it will change the position of the Head. It will use as:

**Syntax:**
```
git reset --soft  
````

## **References :**
---

- https://education.github.com/git-cheat-sheet-education.pdf

- https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud

