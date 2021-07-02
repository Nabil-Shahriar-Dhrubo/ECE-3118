Documentation on Git Commands

Submitted By:
Nabil Shahriar Dhrubo

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
